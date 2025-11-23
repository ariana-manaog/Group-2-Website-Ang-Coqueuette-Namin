from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

@app.route('/profile')
def profile():
    return render_template('profile.html')

@app.route('/works')
def works():
    return render_template('works.html')

@app.route('/contact')
def contact():
    return render_template('contacts.html')

@app.route('/queue')
def queue():
    return render_template('queue.html')

@app.route('/binarytree')
def binarytree():
    return render_template('binarytree.html')

if __name__ == "__main__":
    app.run(debug=True)
