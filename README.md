# Realtime Chat Demo with Laravel 5.4, VueJS, and Pusher

This is just a demo chat app that showcases some of my code base and thought patterns in laravel. This project is by no account a complete project and will be continuously worked on over time.

## Development

1. Clone or fork this repository
2. Run `composer install`
3. Run `php artisan key:generate`
4. Fill out relevant items in your `.env` file (Don't forget to change the broadcasting settings to Pusher), including:
  - DB_CONNECTION
  - PUSHER_APP_ID
  - PUSHER_KEY
  - PUSHER_SECRET
5. Run `npm i`
6. Build assets with `npm run dev`
7. Run `php artisan migrate`
8. Use `php artisan serve` or another method to view the app in the browser
9. **Optional:** Run `php artisan dusk` to run test
