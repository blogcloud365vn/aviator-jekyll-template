---
title: /api/v1/server/{instance_id}/change_password/
position: 2.3
type: post
description: Thay đổi mật khẩu đăng nhập
parameters:
  - name: password
    content: Password muốn thay đổi
  - name: re_password
    content: Nhập lại password muốn thay đổi
right_code_blocks:
  - code_block: |-
        {
          "password": "string",
          "re_password": "string"
        }
    title: Request
    language: json
  - code_block: |-
      {
        "message": string
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





