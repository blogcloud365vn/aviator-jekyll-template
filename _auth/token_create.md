---
title: /books
position: 3.1
type: post
description: Create new token
parameters:
  - name: email
    content: Email login Portal
  - name: password
    content: Password user login Portal
content_markdown: |-
  Token sử dụng cho việc xác thực với Portal
  {: .success}

  Thêm token mới

right_code_blocks:
  - code_block: |-
        {
          "email": "string",
          "password": "string",
          "expired": 0,
          "project_id": "string"
        }
    title: Request
    language: json
  - code_block: |-
      {
        "message": string,
        "token": "string",
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





