<div class="container">
<div class="d-flex justify-content-middle">
<h2>Bootstrap 101!</h2>

<div
  onclick="
    $($('#theme').attr('disabled','disabled')[0].previousElementSibling)
    .attr('disabled','disabled');
  "
  class="btn btn-primary"
>I am a button</div>

---?include=pages/alerts.md
---?include=pages/badges.md
</div>
</div>
