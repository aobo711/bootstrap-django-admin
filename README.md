<h2>Beautiful Django admin template styled with <a href="http://twitter.github.com/bootstrap/">Twitter Bootstrap</a></h2>

<div>Works on Django 1.3 and above.</div>

<h2>Screenshots:</h2>
<div >
    <img src="https://lh5.googleusercontent.com/-YPSx9j0czfg/T2v-QhxTbZI/AAAAAAAAABc/YLo_5nRp6Zo/s433/login.png" />
    <br />
    <img src="https://lh5.googleusercontent.com/-J5YFiMBq6Tc/T2v-PKx3TWI/AAAAAAAAABA/aJWHPIQ7c7s/s1063/home.png" />
    <br />
    <img src="https://lh4.googleusercontent.com/-CirIZtAqdRI/T2v-QI6ikWI/AAAAAAAAABQ/kQz1jEtXPuE/s394/list.png" />
    <br />
    <img src="https://lh4.googleusercontent.com/-ZqZb1Dj4tqc/T2v-PA3ioGI/AAAAAAAAABE/2h04vED09Sc/s543/change_password.png" />
</div>

<h2>How to use:</h2>

<ol>
    <li>Setup django admin first, see https://docs.djangoproject.com/en/dev/ref/contrib/admin/ .</li>
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
</ol>

<h2>Customize Bootstrap</h2>

<div>BootStrap css is under /template/admin/static/css, just rebuild you own bootstrap style, and rewrite bootstrap.css, if might also have to modify rewrite.css.</div>

