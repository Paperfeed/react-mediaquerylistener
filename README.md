# react-mediaquerylistener

A Media Query HOC that adds an fires onChange when the media query triggers

Simply wrap the component you want to monitor with withMediaQueryListener() and pass it a function to the onChange prop. 
The function will fire when a media query triggers.

It automatically creates a MediaQueryList for every breakpoint passed along as prop or uses the default breakpoints you can set in the devices file.


Example onMediaQueryChange function:
```onMediaQueryChange(ev) {
        switch (ev) {
            case 'mobile':
                this.setState({ isCollapsed: true });
                break;
            case 'desktop':
                this.setState({ isCollapsed: false });
        }
    }
```
