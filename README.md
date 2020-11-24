# fileUpload
Without dependency 
 
 
 ### sample
 ```javascript
 <file-upload ref="FileUpload" uploadUrl="/upload/file" uploadKey="uploadfile" :params="{params:1}"
                     :files.sync="images" :singleMode="true" :maxFileSize="2"
                     fileType="image"></file-upload>
 ```
 
 ### priview & add external image to component
 
 ```javascript
 this.$refs.FileUpload.setFiles(
                [
                    {
                        id: 1,
                        path: require('~/assets/media/bg-2.jpg')
                    }
                ]
            );
 ```
 
 ### Props Tables
                    
 Props  | Default  | Type | Example | Description
------------- | ------------- | ------------- | -------------| -------------
uploadUrl  | null |  String | uploadUrl"/api/upload" | 
uploadKey  | uploadfile | String | uploadKey="fileUpload" | 
  params  | null | Object | :params="{ id:1 }" | 
  files.sync  |  | Variable | :files.sync="uploadedList"  | 
   singleMode  |  false | Boolean |  :singleMode="True" | 
   maxFileSize |  2 (mb) | Number |  :maxFileSize="2" | 
   fileType | image | String | fileType="image" |   'image' , 'xls' , 'pdf'
 



## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
