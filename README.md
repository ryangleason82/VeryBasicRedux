## Song Selector

This application is created using the 'Modern React with Redux' course from Udemy. Below are some notes I took throughout the process.

#### Connect

- Reaches back to provider
- Tells the provider about changes to the list of the songs
- If anything changes, the provider will automatically notify the connect function
- The connect function will then pass our list of songs to SongList

#### mapStateToProps

- Says we are going to take all of the data in our redux store
- Run some type of calculation on it to cause data to show up as props in our component
- Can be called anything. Usually called mapStateToProps
- Pass as argument to connect()
  - This is how we get data from the provider

### Flow that will be repeated a million times in every project

- import {connect} from 'react-redux'
- mapStateToProps
- export default connect(mapStateToProps)(YOUR COMPONENT)

#### Misc

- Webpack will automatically give the path of index.js if you don't otherwise specify
- Need curly braces when it's not a defaulted export
