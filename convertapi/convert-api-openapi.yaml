swagger: "2.0"
x-collection-name: ConvertAPI
x-complete: 1
info:
  title: Convert API
  description: the-convertapi-provides-online-api-for-creating-pdf-and-images-from-various-sources-like-word-document-web-pages-or-raw-html-codes--in-just-few-minutes-you-can-integrate-it-into-your-application-and-use-it-easily--return-to-apis-list-
  version: v1
host: do.convertapi.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Email2Image:
    post:
      summary: Email to Image
      description: The API for converting E-Mail files to PDF files and Images. These
        file formats eml, mbx, msg, oft can be converted to png, jpg, tif.
      operationId: email2image
      x-api-path-slug: email2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: eml, mbx, msg, oft'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Email
      - Image
  /Email2Pdf:
    post:
      summary: Email to PDF
      description: The API for converting E-Mail files to PDF files and Images. These
        file formats eml, mbx, msg, oft can be converted to pdf, pdfa, png, jpg, tif.
      operationId: email2pdf
      x-api-path-slug: email2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: eml, mbx, msg, oft'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Email
      - PDF
  /Excel2Image:
    post:
      summary: Excel to Image
      description: The API for converting Excel documents to PDF files and Images.
        These file formats csv, xls, xlsb, xlsx, xlt, xltx can be converted to png,
        jpg, tif.
      operationId: excel2image
      x-api-path-slug: excel2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: csv, xls, xlsb, xlsx, xlt, xltx'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: WorksheetActive
        description: Set to convert active worksheet
      - in: query
        name: WorksheetIndex
        description: Set worksheet index(number) to convert
      - in: query
        name: WorksheetName
        description: Set worksheet name to convert
      responses:
        200:
          description: OK
      tags:
      - Excel
      - Image
  /Excel2Pdf:
    post:
      summary: Excel to PDF
      description: The API for converting Excel documents to PDF files and Images.
        These file formats csv, xls, xlsb, xlsx, xlt, xltx can be converted to pdf,
        pdfa, png, jpg, tif.
      operationId: excel2pdf
      x-api-path-slug: excel2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: csv, xls, xlsb, xlsx, xlt, xltx'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: WorksheetActive
        description: Set to convert active worksheet
      - in: query
        name: WorksheetIndex
        description: Set worksheet index(number) to convert
      - in: query
        name: WorksheetName
        description: Set worksheet name to convert
      responses:
        200:
          description: OK
      tags:
      - Excel
      - PDF
  /Image2Image:
    post:
      summary: Image to Image
      description: The API for converting Image files to PDF files and Images. These
        file formats avs, bmp, dcx, dib, dpx, fax, fits, fpx, gif, ico, iptc, jbig,
        jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv, otb, pbm, pcd, pcds, pct, pcx, pgm,
        pict, png, pnm, ppm, psd, p7, ras, rgba, sun, tga, tiff, tif, vicar, vid,
        viff, wmf, xbm, xpm, xwd can be converted to png, jpg, tif.
      operationId: image2image
      x-api-path-slug: image2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: avs, bmp, dcx, dib, dpx, fax,
          fits, fpx, gif, ico, iptc, jbig, jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv,
          otb, pbm, pcd, pcds, pct, pcx, pgm, pict, png, pnm, ppm, psd, p7, ras, rgba,
          sun, tga, tiff, tif, vicar, vid, viff, wmf, xbm, xpm, xwd'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Image
      - Image
  /Image2Pdf:
    post:
      summary: Image to PDF
      description: The API for converting Image files to PDF files and Images. These
        file formats avs, bmp, dcx, dib, dpx, fax, fits, fpx, gif, ico, iptc, jbig,
        jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv, otb, pbm, pcd, pcds, pct, pcx, pgm,
        pict, png, pnm, ppm, psd, p7, ras, rgba, sun, tga, tiff, tif, vicar, vid,
        viff, wmf, xbm, xpm, xwd can be converted to pdf, pdfa, png, jpg, tif.
      operationId: image2pdf
      x-api-path-slug: image2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: avs, bmp, dcx, dib, dpx, fax,
          fits, fpx, gif, ico, iptc, jbig, jp2, jpeg, jpg, mdi, miff, mng, mpc, mtv,
          otb, pbm, pcd, pcds, pct, pcx, pgm, pict, png, pnm, ppm, psd, p7, ras, rgba,
          sun, tga, tiff, tif, vicar, vid, viff, wmf, xbm, xpm, xwd'
      - in: query
        name: Ocr
        description: Apply optical character recognition (OCR) and convert scanned
          text images into editable and searchable PDF
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Image
      - PDF
  /Journal2Image:
    post:
      summary: Journal to Image
      description: The API for converting Windows Journal Viewer documents to PDF
        files and Images. These file formats jnt can be converted to png, jpg, tif.
      operationId: journal2image
      x-api-path-slug: journal2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: jnt'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Journal
      - Image
  /Journal2Pdf:
    post:
      summary: Journal to PDF
      description: The API for converting Windows Journal Viewer documents to PDF
        files and Images. These file formats jnt can be converted to pdf, pdfa, png,
        jpg, tif.
      operationId: journal2pdf
      x-api-path-slug: journal2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: jnt'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Journal
      - PDF
  /Lotus2Image:
    post:
      summary: Lotus to Image
      description: The API for converting Lotus Smart Suite documents to PDF files
        and Images. These file formats 123, 12m, wk1, wk2, wk3, lwp, mwp, sam can
        be converted to png, jpg, tif.
      operationId: lotus2image
      x-api-path-slug: lotus2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: 123, 12m, wk1, wk2, wk3, lwp,
          mwp, sam'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Lotus
      - Image
  /Lotus2Pdf:
    post:
      summary: Lotus to PDF
      description: The API for converting Lotus Smart Suite documents to PDF files
        and Images. These file formats 123, 12m, wk1, wk2, wk3, lwp, mwp, sam can
        be converted to pdf, pdfa, png, jpg, tif.
      operationId: lotus2pdf
      x-api-path-slug: lotus2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: 123, 12m, wk1, wk2, wk3, lwp,
          mwp, sam'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Lotus
      - PDF
  /OpenOffice2Image:
    post:
      summary: Open Office to Image
      description: The API for converting OpenOffice documents to PDF files and Images.
        These file formats mml, odc, odf, odg, odi, odm, odp, ods, odt, otg, oth,
        otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc, sxg, sxi, sxm, sxw, vor,
        wv2 can be converted to png, jpg, tif.
      operationId: openoffice2image
      x-api-path-slug: openoffice2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: mml, odc, odf, odg, odi, odm,
          odp, ods, odt, otg, oth, otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc,
          sxg, sxi, sxm, sxw, vor, wv2'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Open
      - Office
      - Image
  /OpenOffice2Pdf:
    post:
      summary: Open Office to PDF
      description: The API for converting OpenOffice documents to PDF files and Images.
        These file formats mml, odc, odf, odg, odi, odm, odp, ods, odt, otg, oth,
        otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc, sxg, sxi, sxm, sxw, vor,
        wv2 can be converted to pdf, pdfa, png, jpg, tif.
      operationId: openoffice2pdf
      x-api-path-slug: openoffice2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: mml, odc, odf, odg, odi, odm,
          odp, ods, odt, otg, oth, otp, ots, pxl, sgl, smf, srw, stc, sti, stw, sxc,
          sxg, sxi, sxm, sxw, vor, wv2'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Open
      - Office
      - PDF
  /Pdf2Image:
    post:
      summary: PDF to Image
      description: The API for converting PDF documents to Image. These file formats
        pdf can be converted to png, jpg, tif.
      operationId: pdf2image
      x-api-path-slug: pdf2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: pdf'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - PDF
      - Image
  /Pdf2Pdf:
    post:
      summary: PDF to PDF
      description: The API for converting PDF documents to Image. These file formats
        pdf can be converted to pdf, pdfa, png, jpg, tif.
      operationId: pdf2pdf
      x-api-path-slug: pdf2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: pdf'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - PDF
      - PDF
  /Pdf2PowerPoint:
    post:
      summary: PDF to Power Point
      description: The API for converting PDF documents to PowerPoint presentation
        files. These file formats pdf, pdfa can be converted to pptx.
      operationId: pdf2powerpoint
      x-api-path-slug: pdf2powerpoint-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: pdf, pdfa'
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - PDF
      - Power
      - Point
  /PostScript2Image:
    post:
      summary: Post Script to Image
      description: The API for converting PostScript files to PDF files and Images.
        These file formats ps, eps, prn can be converted to png, jpg, tif.
      operationId: postscript2image
      x-api-path-slug: postscript2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: ps, eps, prn'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Script
      - Image
  /PostScript2Pdf:
    post:
      summary: Post Script to PDF
      description: The API for converting PostScript files to PDF files and Images.
        These file formats ps, eps, prn can be converted to pdf, pdfa, png, jpg, tif.
      operationId: postscript2pdf
      x-api-path-slug: postscript2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: ps, eps, prn'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Script
      - PDF
  /PowerPoint2Image:
    post:
      summary: Power Point to Image
      description: The API for converting PowerPoint documents to PDF files and Images.
        These file formats pot, potx, pps, ppsx, ppt, pptx can be converted to png,
        jpg, tif.
      operationId: powerpoint2image
      x-api-path-slug: powerpoint2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: pot, potx, pps, ppsx, ppt, pptx'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Power
      - Point
      - Image
  /PowerPoint2Pdf:
    post:
      summary: Power Point to PDF
      description: The API for converting PowerPoint documents to PDF files and Images.
        These file formats pot, potx, pps, ppsx, ppt, pptx can be converted to pdf,
        pdfa, png, jpg, tif.
      operationId: powerpoint2pdf
      x-api-path-slug: powerpoint2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: pot, potx, pps, ppsx, ppt, pptx'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Power
      - Point
      - PDF
  /Project2Image:
    post:
      summary: Project to Image
      description: The API for converting Project documents to PDF files and Images.
        These file formats mpp, mpt can be converted to png, jpg, tif.
      operationId: project2image
      x-api-path-slug: project2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: mpp, mpt'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Project
      - Image
  /Project2Pdf:
    post:
      summary: Project to PDF
      description: The API for converting Project documents to PDF files and Images.
        These file formats mpp, mpt can be converted to pdf, pdfa, png, jpg, tif.
      operationId: project2pdf
      x-api-path-slug: project2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: mpp, mpt'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Project
      - PDF
  /Publisher2Image:
    post:
      summary: Publisher to Image
      description: The API for converting Publisher documents to PDF files and Images.
        These file formats pub can be converted to png, jpg, tif.
      operationId: publisher2image
      x-api-path-slug: publisher2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: pub'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Publisher
      - Image
  /Publisher2Pdf:
    post:
      summary: Publisher to PDF
      description: The API for converting Publisher documents to PDF files and Images.
        These file formats pub can be converted to pdf, pdfa, png, jpg, tif.
      operationId: publisher2pdf
      x-api-path-slug: publisher2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: pub'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Publisher
      - PDF
  /RichText2Image:
    post:
      summary: Rich Text to Image
      description: The API for converting Rich Text documents to PDF files and Images.
        These file formats rtf can be converted to png, jpg, tif.
      operationId: richtext2image
      x-api-path-slug: richtext2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: rtf'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Rich
      - Text
      - Image
  /RichText2Pdf:
    post:
      summary: Rich Text to PDF
      description: The API for converting Rich Text documents to PDF files and Images.
        These file formats rtf can be converted to pdf, pdfa, png, jpg, tif.
      operationId: richtext2pdf
      x-api-path-slug: richtext2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: rtf'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Rich
      - Text
      - PDF
  /SnapShot2Image:
    post:
      summary: Snap Shot to Image
      description: The API for converting Access Report Snapshots documents to PDF
        files and Images. These file formats snp can be converted to png, jpg, tif.
      operationId: snapshot2image
      x-api-path-slug: snapshot2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: snp'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Snap
      - Shot
      - Image
  /SnapShot2Pdf:
    post:
      summary: Snap Shot to PDF
      description: The API for converting Access Report Snapshots documents to PDF
        files and Images. These file formats snp can be converted to pdf, pdfa, png,
        jpg, tif.
      operationId: snapshot2pdf
      x-api-path-slug: snapshot2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: snp'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Snap
      - Shot
      - PDF
  /Text2Image:
    post:
      summary: Text to Image
      description: The API for converting Textual files to PDF files and Images. These
        file formats txt, log can be converted to png, jpg, tif.
      operationId: text2image
      x-api-path-slug: text2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: txt, log'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Text
      - Image
  /Text2Pdf:
    post:
      summary: Text to PDF
      description: The API for converting Textual files to PDF files and Images. These
        file formats txt, log can be converted to pdf, pdfa, png, jpg, tif.
      operationId: text2pdf
      x-api-path-slug: text2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: txt, log'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Text
      - PDF
  /Visio2Image:
    post:
      summary: Visio to Image
      description: The API for converting Visio documents to PDF files and Images.
        These file formats vsd, vst, vsdx, vstx can be converted to png, jpg, tif.
      operationId: visio2image
      x-api-path-slug: visio2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: vsd, vst, vsdx, vstx'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Visio
      - Image
  /Visio2Pdf:
    post:
      summary: Visio to PDF
      description: The API for converting Visio documents to PDF files and Images.
        These file formats vsd, vst, vsdx, vstx can be converted to pdf, pdfa, png,
        jpg, tif.
      operationId: visio2pdf
      x-api-path-slug: visio2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: vsd, vst, vsdx, vstx'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Visio
      - PDF
  /Web2Image:
    post:
      summary: Web to Image
      description: The API for converting Web Pages to Images.
      operationId: web2image
      x-api-path-slug: web2image-post
      parameters:
      - in: query
        name: AcceptLanguage
        description: Set accept language header
      - in: query
        name: AlternativeParser
        description: Set alternative parser
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: AuthPassword
        description: HTTP Authentication password, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: AuthUsername
        description: HTTP authentication username, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: ConversionDelay
        description: Delay in seconds before page load and PDF creation
      - in: query
        name: CUrl
        description: URI of a web page to convert
      - in: query
        name: PageHeight
        description: Set screen height
      - in: query
        name: PageWidth
        description: Set screen width
      - in: query
        name: Plugins
        description: Enable plugins such as flash
      - in: query
        name: Scripts
        description: Allow web pages to run javascript
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: UserAgent
        description: Set custom user agent
      responses:
        200:
          description: OK
      tags:
      - Web
      - Image
  /Web2Pdf:
    post:
      summary: Web to PDF
      description: The API for converting Web Pages to PDF files.
      operationId: web2pdf
      x-api-path-slug: web2pdf-post
      parameters:
      - in: query
        name: AcceptLanguage
        description: Set accept language header
      - in: query
        name: AlternativeParser
        description: Set alternative parser
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: AuthPassword
        description: HTTP Authentication password, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: AuthUsername
        description: HTTP authentication username, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: Background
        description: Print web page background
      - in: query
        name: ConversionDelay
        description: Delay in seconds before page load and PDF creation
      - in: query
        name: CoverUrl
        description: Use html document as cover
      - in: query
        name: CUrl
        description: URI of a web page to convert
      - in: query
        name: DocumentTitle
        description: Set the title of the generated pdf file
      - in: query
        name: FooterLine
        description: Display line above the footer
      - in: query
        name: FooterSpacing
        description: Spacing between footer and content
      - in: query
        name: FooterTextCenter
        description: Center aligned footer text
      - in: query
        name: FooterTextFont
        description: Set footer font name
      - in: query
        name: FooterTextLeft
        description: Left aligned footer text
      - in: query
        name: FooterTextRight
        description: Right aligned footer text
      - in: query
        name: FooterTextSize
        description: Set footer font size
      - in: query
        name: FooterUrl
        description: Adds a html footer
      - in: query
        name: HeaderLine
        description: Display line below the header
      - in: query
        name: HeaderSpacing
        description: Spacing between header and content
      - in: query
        name: HeaderTextCenter
        description: Center aligned header text
      - in: query
        name: HeaderTextFont
        description: Set header font name
      - in: query
        name: HeaderTextLeft
        description: Left aligned header text
      - in: query
        name: HeaderTextRight
        description: Right aligned header text
      - in: query
        name: HeaderTextSize
        description: Set header font size
      - in: query
        name: HeaderUrl
        description: Adds a html header
      - in: query
        name: InfoStamp
        description: Show date stamp and conversion url in header
      - in: query
        name: LowQuality
        description: Generates lower quality PDF, makes smaller file size
      - in: query
        name: MarginBottom
        description: Set the page bottom margin
      - in: query
        name: MarginLeft
        description: Set the page left margin
      - in: query
        name: MarginRight
        description: Set the page right margin
      - in: query
        name: MarginTop
        description: Set the page top margin
      - in: query
        name: Outline
        description: Show outline in PDF file
      - in: query
        name: PageHeight
        description: Custom page height
      - in: query
        name: PageNo
        description: Show page number in footer
      - in: query
        name: PageOrientation
        description: 'PDF page orientation: portrait, landscape'
      - in: query
        name: PageSize
        description: PDF page paper sizes
      - in: query
        name: PageWidth
        description: Custom page width
      - in: query
        name: Plugins
        description: Enable plugins such as flash
      - in: query
        name: PrintType
        description: Use print media-type(print css sheet) instead of screen
      - in: query
        name: Scripts
        description: Allow web pages to run javascript
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: UserAgent
        description: Set custom user agent
      responses:
        200:
          description: OK
      tags:
      - Web
      - PDF
  /Word2Image:
    post:
      summary: Word to Image
      description: The API for converting Word documents to PDF files and Images.
        These file formats doc, docx, dot, dotx, wpd, wps, wri can be converted to
        png, jpg, tif.
      operationId: word2image
      x-api-path-slug: word2image-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: doc, docx, dot, dotx, wpd, wps,
          wri'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Word
      - Image
  /Word2Pdf:
    post:
      summary: Word to PDF
      description: The API for converting Word documents to PDF files and Images.
        These file formats doc, docx, dot, dotx, wpd, wps, wri can be converted to
        pdf, pdfa, png, jpg, tif.
      operationId: word2pdf
      x-api-path-slug: word2pdf-post
      parameters:
      - in: query
        name: AlternativeParser
        description: If some objects are missing in converted Pdf files from original
          source files this option can be enabled to improve conversion
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: doc, docx, dot, dotx, wpd, wps,
          wri'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Word
      - PDF
  /Xps2Image:
    post:
      summary: Xps to Image
      description: The API for converting Open XML Paper Specification documents to
        PDF files. These file formats xps can be converted to png, jpg, tif.
      operationId: xps2image
      x-api-path-slug: xps2image-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: File
        description: 'Supported source file formats: xps'
      - in: query
        name: ImageResolutionH
        description: Image horizontal resolution (DPI)
      - in: query
        name: ImageResolutionV
        description: Image vertical resolution (DPI)
      - in: query
        name: JpgQuality
        description: Jpg image quality
      - in: query
        name: OutputFormat
        description: Supported output file formats png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Xps
      - Image
  /Xps2Pdf:
    post:
      summary: Xps to PDF
      description: The API for converting Open XML Paper Specification documents to
        PDF files. These file formats xps can be converted to pdf, pdfa, png, jpg,
        tif.
      operationId: xps2pdf
      x-api-path-slug: xps2pdf-post
      parameters:
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: DocumentAuthor
        description: Set the author of the generated Pdf file
      - in: query
        name: DocumentKeywords
        description: Set the keywords of the generated Pdf file
      - in: query
        name: DocumentSubject
        description: Set the subject of the generated Pdf file
      - in: query
        name: DocumentTitle
        description: Set the title of the generated Pdf file
      - in: query
        name: File
        description: 'Supported source file formats: xps'
      - in: query
        name: OutputFormat
        description: Supported output file formats pdf, pdfa, png, jpg, tif
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      responses:
        200:
          description: OK
      tags:
      - Xps
      - PDF