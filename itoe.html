import pandas as pd
from flask import Flask, render_template_string

# Initialize Flask app
app = Flask(__name__)

# Function to read Excel data
def read_excel_data(filename):
    # Assuming the Excel file has a single sheet
    df = pd.read_excel(filename)
    return df.to_dict(orient='records')

# Route to display data
@app.route('/')
def display_data():
    # Read Excel data
    data = read_excel_data('final.xlsx')
    
    # Render HTML template with data
    template = """
    <html>
    <head>
        <title>OEM's Data</title>
        <style>
        /* Define a colorful style for the h1 heading */
        h1 {
            color: #007bff; /* Blue color */
            text-align: center; /* Center align the heading */
            text-transform: uppercase; /* Convert text to uppercase */
            font-size: 36px; /* Adjust font size */
            /* Add any other styling you want */
        }
    </style>
    </head>
    <body>
        <h1>Hi, Let's have a look at H/W information of all these OEM's</h1>
        <table border="1">
            <tr>
                {% for key in data[0].keys() %}
                    <th>{{ key }}</th>
                {% endfor %}
            </tr>
            {% for row in data %}
                <tr>
                    {% for value in row.values() %}
                        <td>{{ value }}</td>
                    {% endfor %}
                </tr>
            {% endfor %}
        </table>
    </body>
    </html>
    """
    return render_template_string(template, data=data)

if __name__ == '__main__':
    app.run(debug=True)
