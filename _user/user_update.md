---
title: /user
position: 3.2
type: patch
description: Cập nhật thông tin cá nhân của user
parameters:
  - name: first_name
    content: Họ và tên đệm
  - name: last_name
    content: Tên thật
  - name: gender
    content: Giới tính, 1 => Nam, 2 => Nữ, 3=> Cônng ty
  - name: phone_number
    content: Số điện thoại của người sở hữu
  - name: address
    content: Địa chỉ
  - name: company
    content: Tên công ty
right_code_blocks:
  - code_block: |-
        {
          "first_name": "string",
          "last_name": "string",
          "gender": 0,
          "phone_number": "string",
          "address": "string",
          "company": "string"
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





