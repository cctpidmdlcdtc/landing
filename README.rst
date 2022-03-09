python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 app.py

The first time you run this example, a sample sqlite database gets populated automatically. To suppress this behaviour,
comment the following lines in app.py:::

     if not os.path.exists(database_path):
         build_sample_db()
