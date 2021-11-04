---
title: contact
---
<div class="contact-container">
  <p>tokyo-based work inquiries</p>
  <a id="b64-email">contact via email</a>
</div>
<script>
  // Mitigate some spam
  var email = "{{ site.social.email }}";
  document.getElementById("b64-email").href = `mailto:${atob(email)}`;
</script>
