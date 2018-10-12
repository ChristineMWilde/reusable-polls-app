=====
Polls
=====
 
Polls is a reusable voting app for Django which can be used in conjunction with the threads/forum app found here under the 'forum/threads app<https://github.com/ChristineMWilde/reusable-threads-app.git>'_.
 
Detailed documentation is in the "ProjectDocumentation" directory.
 
Quick start
-----------
 
1. The polls app is dependent on the threads app. Please first download the threads app. Download link:

2. Add 'reusable_polls' to your INSTALLED_APPS setting like this::
 
    INSTALLED_APPS = (
        ...
        'reusable_polls',
    )
 
2. Ensure to include the voting URLconf for your project in the threads app urls.py like this::
 
    url(r'^thread/vote/', include('reusable_threads.urls')), *within the threads app
 
3. Run `python manage.py migrate` to create the polls models.
 
