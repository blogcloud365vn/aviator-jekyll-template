---
title: Server List IP
position: 2.12
type: get
description: /api/v1/server/{instance_id}/list_ip/
left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/server/{instance_id}/list_ip/',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        method: 'GET',
        success: function(data){
          console.log(data);
        }
      });
    title: jQuery
    language: javascript
  - code_block: |-
      r = requests.get("/api/v1/server/{instance_id}/list_ip/", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
right_code_blocks:
  - code_block: |-
      [
        {
          "fixed_ips": [
            {
              "subnet_id": "string",
              "ip_address": "string"
            }
          ],
          "mac_address": "string",
          "is_public": false,
          "port_id": "string"
        }
      ]

    title: Response
    language: json
---