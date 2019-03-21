@channel:
1) unzip where you want it, run `npm install` to get node modules.
2) `npm start` to get onscreen. You should get live updates (let us know if you get any file watcher errors)
3) it won't work! You're trying to render a React object. Trace where the error is happening and change what is rendered.
4) addBucket won't work either - you're trying to add a string to a list of objects. Change what you set to state in addBucket.
5) replace the removeBucket function with a `toggleBucketAcquired` function that changes the array of buckets so that one of them has the acquired property flipped true/false. Remember, you can't mutate _anything_.
6) use this acquired property in some way - think how you could conditionally apply class names and import some CSS to show this is some way.
7) extend your data/behaviour in some way - up to you how! Possibilities include adding sortable dates, priorities, categories...