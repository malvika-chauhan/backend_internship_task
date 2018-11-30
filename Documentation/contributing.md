# Contribution guide


## Workflow

We follow gitflow workflow.

However, there will be no direct push to master branch of main repository `https://github.com/`. <br>
All the changes will be committed on a branch named `<your-username>`. And then you've to create a pull request to development branch of main repository `https://github.com/`.
Create a pull request as soon as you're finished with a feature. Don't shy. If required, we will give you advice to improve your PR, or else we will merge it.

## Prerequisite

Basic understanding of Laravel.

Your system must have:

- Git (mandatory)
- PHP (mandatory)
- Composer (mandatory)


## Setting project locally

### Checkout main repo.

```bash
git clone https://github.com/
git checkout -b <your-username>
```


### Copy .env

We need to make a copy of `.env.example` as `.env`

```bash
cd laravel-task
cp .env.example .env
```

After that, edit `.env` file with database settings. You need to create empty database and update .env file.

### Composer install

(Prerequisite, composer installed. )
We use composer to install all dependencies, running the following command: 

```bash
composer install
```

### Generating keys

Laravel uses an unique key for its internal encryption feature and we need to generate it, by running the following command:

```bash
php artisan key:generate
```

### Adding remote upstream

Some key terms:

- Laravel Task repo: Main repository https://github.com/
- remote: Git specific term to represent different repository.
- origin: Default remote of git. On your checkout, it will represent your fork.
- PR (pull request): It's you asking the Zomeds Internship Module Repo to review and accept/reject your modifications.


There are many tutorial/articles available for that but if you still have doubts, please email us at `tech@zomeds.in`


```bash
git checkout master
git pull origin master
git checkout development
git pull origin development
git checkout <your-username>
```

Now create the feature and test it locally. Once you think it is working properly, and you are ready to send PR, get update to avoid any merge conflict in PR.

```bash
git add <all new/modified files>
git commit -m "<message>"
git checkout development
git pull origin development
git checkout <your-username>
git merge development
git push origin <your-username>
```

Great, now open up your favorite IDE and start finishing your tasks. Please make sure you send PR to development branch on the main repo.
