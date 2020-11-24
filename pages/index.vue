<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12 d-flex align-items-center justify-content-center vh-100">
        <file-upload uploadUrl="/upload/file" uploadKey="uploadfile" :params="{params:1}"
                     :files.sync="images"  :maxFileSize="2"
                     fileType="image"></file-upload>
      </div>
    </div>
  </div>
</template>

<script>
  import fileUpload from "@/components/fileUpload";

  export default {
    components: {fileUpload},
    data: () => ({
      images: []
    })

  }
</script>

<style>

</style>
