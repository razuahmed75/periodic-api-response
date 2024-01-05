If you want to call the API regardless of whether the widget is rebuilt or not, and you want to continuously check for changes in the API response, you might consider using a periodic task like a timer. Here's an example using the Timer class to periodically fetch data:
------------------------------------

This example introduces a periodic timer in the ApiProvider constructor that triggers the fetchData method at regular intervals. Adjust the _fetchInterval based on how frequently you want to check for changes in the API response. The timer is canceled in the dispose method to clean up resources when the provider is no longer needed.

Keep in mind that frequent API polling may have performance and efficiency considerations, so it's important to choose an appropriate interval based on your specific use case.
