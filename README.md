# Stripe-Checkout-server using Flask Python



https://testdriven.io/blog/flask-stripe-tutorial/.

Follow the tutorial in the link to setup a Stripe account. It will be required to gain your secret and published keys

Make sure you have the correct python environments. I installed pyenv to have multiple python versions on a mac,
and switched to version 3.10.2.

1. Create and activate a virtual environment:

    ```sh
    $ python3 -m venv venv && source venv/bin/activate
    ```

1. Install Flask and stripe:

    ```sh
    (venv)$ pip install flask
    (venv)$ pip install stripe
    ```


1. Before this next step, make sure to register a Stripe account. Add your Stripe test secret and publishable keys as environment variables like so:

    ```sh
    (venv)$ export STRIPE_PUBLISHABLE_KEY=<YOUR_STRIPE_PUBLISHABLE_KEY>
    (venv)$ export STRIPE_SECRET_KEY=<YOUR_STRIPE_SECRET_KEY>
    (env)$ export STRIPE_ENDPOINT_SECRET=<YOUR_ENDPOINT_SECRET_KEY>
    ```

1. Run the server:

    ```sh
    (venv)$ FLASK_ENV=development python app.py
    ```

    Navigate to [http://localhost:5000](http://localhost:5000).
