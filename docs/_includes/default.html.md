<!DOCTYPE html>
<html lang="{{ site.lang | default: 'en-US' }}">
  {% include head.html %}
  <body class="layout-{{ page.layout | default: 'default' }}">
    {% include components/header.html %}
    {% include components/breadcrumbs.html %}
    <main id="main-content" class="main-content" aria-label="Content">
      <div class="page-content">
        {{ content }}
      </div>
    </main>
    {% include components/footer.html %}
    {% include scripts.html %}
  </body>
</html>