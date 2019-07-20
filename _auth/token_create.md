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
# left_code_blocks:
#   - code_block: |-
#       $.post("http://192.168.70.65/api/v1/auth/tokens", {
#         "token": "YOUR_APP_KEY",
#         "title": "The Book Thief",
#         "score": 4.3
#       }, function(data) {
#         alert(data);
#       });
#     title: jQuery
#     language: javascript
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





