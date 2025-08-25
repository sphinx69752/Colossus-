# Colossus-
Arcade center
from flask import Flask
import os

app = Flask(__name__)

@app.route("/")
def home():
    return "Colossus v1 - Déploiement minimal OK !"

if __name__ == "__main__":
    port = int(os.environ.get("PORT", 10000))
    app.run(host="0.0.0.0", port=port)

