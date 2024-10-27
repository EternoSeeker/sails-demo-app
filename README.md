## ⛵ A [Sails.js](https://sailsjs.com) web app with UI tests. ✅

<p align="left"><a href="https://github.com/mdmintz/sails-demo-app/blob/master/ui_tests/test_sails_app.py"><img src="https://seleniumbase.io/cdn/gif/sails_app_gif.gif" alt="SeleniumBase Test for the SailsJS Demo App" title="SeleniumBase Test for the SailsJS Demo App" width="400" /></a></p>

#### ⛵ Complete the server

```bash
npm install
```

#### ⛵ Starting the server

```bash
node app.js
# - OR - #
sails lift
```

#### ⛵ [http://localhost:1337](http://localhost:1337)

(The app will stay up while the server is running.)

### Test Environment Setup / Running Tests

(In a separate terminal / command prompt.)

#### 🔵 Go to the ``ui_tests/`` folder:

```bash
cd ui_tests/
```

#### 🔵 Create a Python virtual environment:

```bash
# Linux / macOS instructions
python3 -m venv sbase_env
source sbase_env/bin/activate

# Windows instructions
py -m venv sbase_env
call sbase_env\\Scripts\\activate
```

#### 🔵 Install SeleniumBase + Chromedriver

```bash
pip install seleniumbase --upgrade
seleniumbase install chromedriver
```

#### 🔵 Run the tests

```bash
pytest -v --rs --crumbs --dashboard
```

✅ Here's what all those options do:

* ``-v`` : Display each test on a separate line.
* ``--rs`` : Reuse the browser session between tests.
* ``--crumbs`` : Clear cookies between tests using ``--rs``.
* ``--dashboard`` : Output test results to ``dashboard.html``.
