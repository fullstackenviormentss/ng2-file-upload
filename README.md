# ngx-file-upload [![npm version](https://badge.fury.io/js/ngx-file-upload.svg)](http://badge.fury.io/js/ngx-file-upload) [![npm downloads](https://img.shields.io/npm/dm/ngx-file-upload.svg)](https://npmjs.org/ngx-file-upload)[![slack](https://ngx-slack.herokuapp.com/badge.svg)](https://ngx-slack.herokuapp.com)
Easy to use Angular directives for files upload ([demo](http://valor-software.github.io/ngx-file-upload/))

[![Angular Style Guide](https://mgechev.github.io/angular2-style-guide/images/badge.svg)](https://github.com/mgechev/angular2-style-guide)
[![Build Status](https://travis-ci.org/valor-software/ngx-file-upload.svg?branch=development)](https://travis-ci.org/valor-software/ngx-file-upload)
[![Dependency Status](https://david-dm.org/valor-software/ngx-file-upload.svg)](https://david-dm.org/valor-software/ngx-file-upload)

## Quick start

1. A recommended way to install ***ngx-file-upload*** is through [npm](https://www.npmjs.com/search?q=ngx-file-upload) package manager using the following command:

  `npm i ngx-file-upload --save`

  Alternatively, you can [download it in a ZIP file](https://github.com/valor-software/ngx-file-upload/archive/master.zip).

2. Currently `ngx-file-upload` contains two directives: `ngx-file-select` and `ngx-file-drop`. `ngx-file-select` is used for 'file-input' field of form and
  `ngx-file-drop` is used for area that will be used for dropping of file or files.

3. More information regarding using of ***ngx-file-upload*** is located in
  [demo](http://valor-software.github.io/ngx-file-upload/) and [demo sources](https://github.com/valor-software/ngx-file-upload/tree/master/demo).

## API for `ngxFileSelect`

### Properties

  - `uploader` - (`FileUploader`) - uploader object. See using in [demo](https://github.com/valor-software/ngx-file-upload/blob/master/demo/components/file-upload/simple-demo.ts)

## API for `ngxFileDrop`

### Properties

  - `uploader` - (`FileUploader`) - uploader object. See using in [demo](https://github.com/valor-software/ngx-file-upload/blob/master/demo/components/file-upload/simple-demo.ts)

  Parameters supported by this object:

  1. `url` - URL of File Uploader's route
  2. `authToken` - Auth token that will be applied as 'Authorization' header during file send.
  3. `disableMultipart` - If 'true', disable using a multipart form for file upload and instead stream the file. Some APIs (e.g. Amazon S3) may expect the file to be streamed rather than sent via a form. Defaults to false.
  4. `itemAlias` - item alias (form name redefenition)

### Events

  - `fileOver` - it fires during 'over' and 'out' events for Drop Area; returns `boolean`: `true` if file is over Drop Area, `false` in case of out.
  See using in [ts demo](https://github.com/valor-software/ngx-file-upload/blob/master/demo/components/file-upload/simple-demo.ts) and
  [html demo](https://github.com/valor-software/ngx-file-upload/blob/master/demo/components/file-upload/simple-demo.html)

# Troubleshooting

Please follow this guidelines when reporting bugs and feature requests:

1. Use [GitHub Issues](https://github.com/valor-software/ngx-file-upload/issues) board to report bugs and feature requests (not our email address)
2. Please **always** write steps to reproduce the error. That way we can focus on fixing the bug, not scratching our heads trying to reproduce it.
3. Opened issues not related to this repository will be periodically closed. We suggest you use StackOverflow to ask these question.

Thanks for understanding!

### License

The MIT License (see the [LICENSE](https://github.com/valor-software/ngx-file-upload/blob/master/LICENSE) file for the full text)
