---
title: /server/{instance_id}/rename/
position: 2.9
type: post
description: Đổi tên máy chủ ảo
parameters:
  - name: server_name
    content: Tên máy chủ ảo muốn thay đổi
right_code_blocks:
  - code_block: |-
        {
          "server_name": "string"
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
