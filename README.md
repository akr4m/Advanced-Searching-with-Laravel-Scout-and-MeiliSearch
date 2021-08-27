## Advanced Searching with Laravel Scout and MeiliSearch

- Laravel
- Laravel Scout
- MeiliSearch

Demo Project of An Advanced Searching with Laravel Scout and MeiliSearch

### Routes

```php

Route::get('/', function () {
    return view('welcome');
});

Route::get('/dashboard', function () {
    return view('dashboard');
})->middleware(['auth'])->name('dashboard');

Route::get('/search', SearchController::class);

Route::get('/update', function () {
    Article::find(64)->update([
        'title' => 'A new title!'
    ]);
});

require __DIR__.'/auth.php';

```
