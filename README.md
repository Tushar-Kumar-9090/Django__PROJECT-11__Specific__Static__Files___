# Django__PROJECT-11__Specific__Static__Files___

SPECIFIC STATIC FILE OR SPECIFIC STATIC FOLDER

HERE we have to create 2 static folder
    -->one static folder we have to create inside project11 and in this static folder we store css and js file
    -->one static folder we have to create inside app and in this static folder we store only images

ANOTHER static folder automatically created by DJANGO in outer project

-------------------------------------------------------------------------------------------------------------------------

We have to create this in setting.py---->>>
      import os
      TEMPLATE_DIR = os.path.join(BASE_DIR, 'templates')
      STATIC_DIR_project11 = os.path.join(os.path.join(BASE_DIR, 'project11'),'static')
      STATIC_DIR_app = os.path.join(os.path.join(BASE_DIR, 'app'),'static')
      STATIC_ROOT = os.path.join(BASE_DIR, 'static')
      STATICFILES_DIRS = [STATIC_DIR_project11,STATIC_DIR_app]
      
-------------------------------------------------------------------------------------------------------------------------


for accessing images by using  <img> and inside src use jinja tag and then we can access images

for accessing css by using <link> and inside href use jinja tag and then we can access css files
