from flask import Flask

app = Flask(__name__)

@app.route('/')  # This decorator associates the following function with the '/' route
def index():
    return 'Hello, World!'

@app.route('/about')  # This decorator associates the following function with the '/about' route
def about():
    return 'About Page'

if __name__ == '__main__':
    app.run(debug=True)

