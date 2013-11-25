

<h3>Django admin templates styled with <a href="http://twitter.github.com/bootstrap/">Twitter Bootstrap 3</a></h3>
<div>Work with Django 1.5 and BootStrap 3</div>

<h2>Screenshots:</h2>
<div >

    <img src="https://lh5.googleusercontent.com/-YPSx9j0czfg/T2v-QhxTbZI/AAAAAAAAABc/YLo_5nRp6Zo/s433/login.png" />
    <br />
    <img src="https://lh4.googleusercontent.com/-Oc1soVl6QF0/UDcW3OpYwFI/AAAAAAAAAFA/E22PV_sbH24/s741/login.png" />
    <br />
    <img src="https://lh4.googleusercontent.com/-1YuZPYz9MzA/UDcW19Vl9rI/AAAAAAAAAE4/W75RsC_htkM/s741/list.png" />
    <br />
    <img src="https://lh6.googleusercontent.com/-HUFdhCXBuPE/UDcWy_S3zrI/AAAAAAAAAEo/z8_elmA_HAc/s741/change.png" />
    <br />
    <img src="https://lh5.googleusercontent.com/-o6kjfc7p4yk/UDcW0jd9nuI/AAAAAAAAAEw/g2dmD3h4AUU/s567/add.png" />
    <br />
</div>

<h2>Get Started:</h2>

<ol>
    <li>Setup django admin first, link: <a href="https://docs.djangoproject.com/en/dev/ref/contrib/admin/">https://docs.djangoproject.com/en/dev/ref/contrib/admin/</a> .</li>
    <li>Put <code>admin_bootstrap</code> directory in your project directory or elsewhere in your <code>sys.path</code>.</li>
    <li>Add <code>admin_bootstrap</code> to <code>INSTALLED_APPS</code> in <code>settings.py</code>, before <code>django.contrib.admin</code>.</li>
    <li>Run <code>./manage.py collectstatic</code>(requested to collect static files at the destination location as <code>STATIC_ROOT</code>).</li>
</ol>

<h2>Customize Bootstrap</h2>

<div>BootStrap css is at <code>/admin_bootstrap/static/css</code>, rewrite styles and build yours.</div>

