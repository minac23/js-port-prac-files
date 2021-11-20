<Switch>
    <Route path='/home' component={HomePage} />
    <Route exact path='/directory' render={() => <Directory campsites={this.state.campsites} />} />
    <Route path='/directory/:campsiteId' component={CampsiteWithId} />
    <Route exact path='/contactus' component={Contact} />
    <Redirect to='/home' />
</Switch>


# need to import "react-router-dom"
import { BrowserRouter, Route} from "react-router-dom";

# place <BrowserRouter> in App (does not have to be but this way in parent and can access children components)

<BrowserRouter>
    <Route path='/' component={Home} />
    <Route path='/aboutus' component={} />
</BrowserRouter>

# import {component} into the App
import {Home} from "./Home";

# 
React will match all the paths that "match" unless you use "exact"




