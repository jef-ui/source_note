### Config GIT & GITHUB + Cloning

cd /opt/lamp/htdocs/

>>sudo git clone <https_code_repo_project_url> note: this command is from your repo project in your github profile (https)

>> open the folder repo and code . (to open vs code)

>>Edit the .env file base on your password and user 

>>if you can't save it type this command (sudo chown -R USERNAME:USERNAME /opt/lampp/htdocs/projectname)

>>composer install and npm install

>>copy .env example and rename it to .env

>>php artisan migrate

>>php artisan key:generate

>>npm run build

>>php artisan serve

>>git config --global user.email "your-email"

>>git config --global user.name "your.name"

>>git remote set-url origin https://<token>@github.com/<user.name>/<repo.name>
