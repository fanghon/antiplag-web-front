<template>
  <div class="modal fade" id="helpModalCenter" tabindex="-1" role="dialog" aria-labelledby="helpModalCenterTitle"
       aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered modal-lg" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="helpModalCenterTitle">欢迎使用本系统</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
          <div class="alert alert-light" role="alert">
            <p>网页版作业查重系统</p>
            <hr>
            <ul class="ml-4">
              <li><span style="color: crimson">代码查重步骤</span>
                <ul class="ml-4">
                  <li>获取学生作业</li>
                  <li>将所有学生作业解压到单独的文件夹</li>
                  <li>上传母文件夹到查重系统中</li>
                  <li>选择作业中的编程语言，和抄袭阈值，一般建议阈值从50开始，选择moss则没有阈值设置</li>
                  <li>待上传完成后，点击执行比较按钮，耐心等待，一般不超过半分钟</li>
                  <li>计算完成后，点击右下角的查看详细结果，然后进行比对</li>
                </ul>
              </li>
              <li>文件管理
                <ul class="ml-4">
                  <li>左侧为文件上传部分，支持多文件上传、文件夹上传方式，支持取消、断点续传、失败重试操作。可进行多次上传操作。</li>
                  <li>建议上传文件夹，该文件夹内按照学生分子文件夹，直接上传即可</li>
                  <li>中间为管理已上传到服务器文件部分。</li>
                  <li>如果删除文件后需要重新上传同一文件，请先清除左侧记录。</li>
                </ul>
              </li>
              <li>文本查重
                <ul class="ml-4">
                  <li>对于文档，与代码类似，上传过后系统会自动转成txt进行比较，支持word、PDF等格式</li>
                </ul>
              </li>

            </ul>
          </div>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-outline-dark btn-sm" data-dismiss="modal">关闭</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "help"
}
</script>

<style lang="less" scoped>
.no-box-shadow:focus {
  box-shadow: none !important;
}
</style>