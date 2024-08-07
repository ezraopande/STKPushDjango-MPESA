# STKPushDjango-MPESA

A Django application for integrating M-Pesa STK Push functionality.

## Features

- Initiate M-Pesa STK Push transactions
- Handle transaction callbacks
- View transaction status and details

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/ezraopande/STKPushDjango-MPESA.git
    ```
2. Navigate to the project directory:
    ```sh
    cd STKPushDjango-MPESA
    ```
3. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```


## Configuration

1. Create a `.env` file in the root of the project and add your M-Pesa API credentials:
    ```sh
    MPESA_CONSUMER_KEY=<your_consumer_key>
    MPESA_CONSUMER_SECRET=<your_consumer_secret>
    MPESA_SHORTCODE=<your_shortcode>
    MPESA_PASSKEY=<your_passkey>
    CALLBACK_URL=<your_callback_url>
    ```

2. Apply the database migrations:
    ```sh
    python manage.py migrate
    ```

3. Create a superuser to access the Django admin:
    ```sh
    python manage.py createsuperuser
    ```

## Usage

1. Start the Django development server:
    ```sh
    python manage.py runserver
    ```

2. Access the application at `http://127.0.0.1:8000/`.

## Endpoints

- `/stk_push/`: Endpoint to initiate an STK Push transaction.
- `/callback/`: Endpoint to handle M-Pesa callback.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


## Contact

For any questions or feedback, feel free to reach out to:

- Email: ezraopande@gmail.com
- Phone: +254796759850

---

*This project is maintained by [Ezra Opande](https://github.com/ezraopande).*
