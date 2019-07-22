---
title: Token Create
position: 1.1
type: post
description: Create new token
parameters:
  - name: email
    content: Email sử dụng để đăng nhập portal
  - name: password
    content: Password sử dụng để đăng nhập portal
  - name: expired
    content: Thời gian tồn tại của token (tính bằng giờ)
content_markdown: |-
  Token sử dụng cho việc xác thực với Portal
  /api/v1/auth/tokens
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
        "message": "string",
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





