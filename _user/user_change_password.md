---
title: /user
position: 3.3
type: post
description: Thay đổi mật khẩu truy cập của user
parameters:
  - name: old_password
    content: Mật khẩu cũ
  - name: new_password
    content: Mật khẩu mới muốn thay đổi
  - name: re_password
    content: Nhập lại mật khẩu muốn thay đổi
right_code_blocks:
  - code_block: |-
        {
          "old_password": "string",
          "new_password": "string",
          "re_password": "string"
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





