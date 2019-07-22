---
title: Token Delete
position: 1.3
type: delete
description: /api/v1/auth/tokens

left_code_blocks:
  - code_block: |-
      $.ajax({
        url: '/api/v1/auth/tokens',
        headers: {
            'Authorization':'Token $TOKEN',
        },
        type: 'DELETE',
          success: function(result) {}
      });
    title: jQuery
    language: javascript
  - code_block: |-
      r = requests.delete("/api/v1/auth/tokens", token="YOUR_TOKEN_KEY")
      print r.text
    title: Python
    language: python
---