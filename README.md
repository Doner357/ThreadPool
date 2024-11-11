Taco::ThreadPool
==========

A simple C++17 Thread Pool implementation.
Fork and modified version of [progschj/ThreadPool](https://github.com/progschj/ThreadPool?tab=Zlib-1-ov-file)

Basic usage:
```c++
// create thread pool with 4 worker threads
taco::ThreadPool pool(4);

// enqueue and store future
auto result = pool.enqueue([](int answer) { return answer; }, 42);

// get result from future
std::cout << result.get() << std::endl;

```
