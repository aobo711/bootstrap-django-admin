<h2>Beautiful Django admin template styled with <a href="http://twitter.github.com/bootstrap/">Twitter Bootstrap</a></h2>

<div>Bootstrap 2.0 Upgraded.</div>
<div>Works on Django 1.3 and above.</div>

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

<h2>How to use:</h2>

<ol>
    <li>Setup django admin first, link: <a href="https://docs.djangoproject.com/en/dev/ref/contrib/admin/">https://docs.djangoproject.com/en/dev/ref/contrib/admin/</a> .</li>
    <li>Clone the project to you workspace, copy the template folder to you django project root, so the template will locates at the same directory as settings.py. </li>
    <li>Modify settings:
        <ol>
            <li>Add 
                <code>
                    os.path.join(os.path.dirname(__file__), 'templates').replace('\\', '/')
                </code>
                to TEMPLATE_DIRS in settings.py.
            </li>
            <li>
                Add additional url rule to urls.py, this rule is used for hosting static resouce in admin templates:
                <pre >
                (r'^admins/(?P<path>.*)$', 'django.views.static.serve', {'document_root': '/your_project_directory/project_name/project_folder/templates/admin/static', 'show_indexes': True}),
                </pre>
                Github hides tag 'path', so you need to add it after '(?P', or find it in change log.
            </li>
        <ol>
    </li>
</ol>

<h2>Customize Bootstrap</h2>

<div>BootStrap css locates at /template/admin/static/css, rewrite styles and rebuild, you can also modify rewrite.css.</div>

