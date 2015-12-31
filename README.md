# Happyr LinkedIn bundle

This is a very small bundle that registers a service for the [LinkedIn client](https://github.com/Happyr/LinkedIn-API-client).
Usage: 

```yaml
happyr_linkedin:
  app_id: 'xxx'
  app_secret: 'yyy'
```

```php
$linkedin = $this->get('happyr.linkedin');
$user = $linkedin->get('v1/people/~:(firstName,lastName)');
```

For more info look at the libraries repository: https://github.com/Happyr/LinkedIn-API-client

### Authentication

The easiest way to implement LinkedIn Authentication is to use Symfony's Guard component. 