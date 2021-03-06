#Async Event Bus
=============================

An Guava-based event bus tailored for the Android.

API and some code forked from the Google Guava.

The Async Event Bus uses threads to offload work from the UI thread - the most 
important thread for Android applications. By default all events are 
dispatched in one of the background thread, then optionally delivered to subscribers 
in many different threads, according to subscriber needs. Yes, subscriber needs, 
because subscriber can define which thread it will be called. 

Because of asynchronous processing, posting an event is very cheap for 
the posting thread. Also events can be easily used for cross-thread communication, 
ex. to deliver the result of the background calculation or the network query 
directly to the UI thread.


License
-------

Copyright 2015 Łukasz Płomiński 

Copyright 2010 Google, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.