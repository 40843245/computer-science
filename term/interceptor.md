# interceptor
## Intro
Interceptors are a powerful mechanism that can monitor, rewrite, and retry calls.

## Example

Here’s a Java code about simple interceptor that logs the outgoing request and the incoming response (from [interceptors](https://square.github.io/okhttp/features/interceptors/)

```
class LoggingInterceptor implements Interceptor {
  @Override public Response intercept(Interceptor.Chain chain) throws IOException {
    Request request = chain.request();

    long t1 = System.nanoTime();
    logger.info(String.format("Sending request %s on %s%n%s",
        request.url(), chain.connection(), request.headers()));

    Response response = chain.proceed(request);

    long t2 = System.nanoTime();
    logger.info(String.format("Received response for %s in %.1fms%n%s",
        response.request().url(), (t2 - t1) / 1e6d, response.headers()));

    return response;
  }
}
```

## Diagram
<img width="600" alt="interceptors@2x" src="https://github.com/user-attachments/assets/9f5e066a-ae8c-4a0b-9362-8e7ff1304c49">

## Ref
+ [Interceptor (square.github.io)](https://square.github.io/okhttp/features/interceptors/)
+ [Interceptor pattern (Wiki)](https://en.wikipedia.org/wiki/Interceptor_pattern)
