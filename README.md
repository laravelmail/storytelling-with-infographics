# Storytelling With Infographics

This newsletter showcases the power of storytelling through infographics, demonstrating how data can be visually engaging and easy to understand across various industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Technology, Education
- **Message Type:** Newsletter
- **Tags:** storytelling, infographics

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/storytelling-with-infographics.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/storytelling-with-infographics/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.storytelling-with-infographics',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
