<h2>Beautiful Django admin template styled with <a href="http://twitter.github.com/bootstrap/">Twitter Bootstrap</a></h2>

<div>Works on Django 1.3 and above.</div>

<h2>How to use:</h2>

<ol>
    <li>Setup django admin first, see https://docs.djangoproject.com/en/dev/ref/contrib/admin/</li>
    <li>Clone the project to you workspace, copy the template folder to you django project root, so the template located the same directory as settings.py. </li>
    <li>Modify settings:
        <ol>
            <li>Add 
                <code>
                    os.path.join(os.path.dirname(__file__), 'templates').replace('\\','/')
                </code>
                to TEMPLATE_DIRS in settings.py.
            </li>
            <li>
                Add additional url rule to urls.py, we use it in hosting static resouce in admin templates:
                <code >
                (r'^admins/(?P<path>.*)$', 'django.views.static.serve', {'document_root': '/your_project_directory/project_name/project_folder/templates/admin/static', 'show_indexes': True}),
                </code>
            </li>
        <ol>
    </li>
<ol>

<h2>Customize Bootstrap</h2>

<div>BootStrap css is under /template/admin/static/css, just rebuild you own bootstrap style, and rewrite bootstrap.css, if might also have to modify rewrite.css.</div>

