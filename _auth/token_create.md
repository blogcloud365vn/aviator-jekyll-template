---
title: Token Create
position: 1.1
type: post
description: /api/v1/auth/tokens
parameters:
  - name: email
    content: Email sử dụng để đăng nhập portal
  - name: password
    content: Password sử dụng để đăng nhập portal
  - name: expired
    content: Thời gian tồn tại của token (tính bằng giờ)
left_code_blocks:
  - code_block: |-
      $.post("/api/v1/auth/tokens", {
        "email": "user@example.com",
        "password": "string"
      }, function(data) {
        console.log(data);
      });
    title: jQuery
    language: javascript
  - code_block: |-
      data = { 'username' : 'user@example.com', 'password' : 'string' }
      r = requests.post('/api/v1/auth/tokens', data=json.dumps(data), verify=False)
      token = json.loads(r.text)
    title: Python
    language: python

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





