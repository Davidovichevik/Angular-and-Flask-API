# Angular-and-Flask-API
Full-Stack Web Application with Angular and Flask API:
// app.component.ts (Angular)
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  template: '<h1>Hello, Angular!</h1>',
})
export class AppComponent {}

// app.py (Flask API)
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return {'message': 'Hello, Flask API!'}

if __name__ == '__main__':
    app.run(debug=True)
