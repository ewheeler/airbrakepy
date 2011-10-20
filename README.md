Pulse Energy AirbrakePy
==========================
AirbrakePy provides a logging.Handler implementation that can be configured to alert Airbrake (http://airbrakeapp.com).

(c) 2011 Pulse Energy, Inc.

To use with Flask:
==================
from airbrakepy.logging.handlers import AirbrakeHandler
handler = AirbrakeHandler('my-key', environment='production', component_name='my-flask-app', node_name='my-node-name')

app = Flask(__name__)
app.logger.addHandler(handler)
