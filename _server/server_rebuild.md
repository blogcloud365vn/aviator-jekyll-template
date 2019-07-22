---
title: /server/{instance_id}/rebuild/
position: 4.10
type: post
description: Thay đổi hệ điều hành của máy chủ ảo
parameters:
  - name: os_image
    content: ID của hệ điều hành muốn thay đổi
right_code_blocks:
  - code_block: |-
        {
          "os_image": 0
        }
    title: Request
    language: json
  - code_block: |-
      {
        "message": "string"
      }
    title: Response
    language: json
  - code_block: |-
      {
        "error": true,
        "message": "string"
      }
    title: Error
    language: json
---
