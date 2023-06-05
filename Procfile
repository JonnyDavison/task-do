 web: python run.py

 app = Flask(__name__)
 app.config["SECRET_KEY"] = os.environ.get("SECRET_KEY")

 if os.environ.get("DEVELOPMENT") == "True":
     app.config["SQLALCHEMY_DATABASE_URI"] = os.getenv("DATABASE_URI")
     app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get("DB_URL")
 else:
     app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get("DATABASE_URL")


if os.environ.get("DEVELOPMENT") == "True":
     app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get("DB_URL")
 else:
     uri = os.environ.get("DATABASE_URL")
     if uri.startswith("postgres://pffcwzwr:syNUm3en877GlwAHMREaVVGr_vKidRUQ@lucky.db.elephantsql.com/pffcwzwr"):
         uri = uri.replace("postgres://pffcwzwr:syNUm3en877GlwAHMREaVVGr_vKidRUQ@lucky.db.elephantsql.com/pffcwzwr", "postgres://pffcwzwr:syNUm3en877GlwAHMREaVVGr_vKidRUQ@lucky.db.elephantsql.com/pffcwzwr", 1)
     app.config["SQLALCHEMY_DATABASE_URI"] = uri     