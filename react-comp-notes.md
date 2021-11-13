# need to import React
import React, {Component} frpm 'react;

class Directory extends Component {
    constructor(props) {
        super(props);
        this.state = {}; //empty object
    } 
    render(){
        return (

        );
    }
}

# attempt 1
if(this.props.campsite) {
            return (
                <div className="row" />
            );
        }
        return <div />;
        }

# attempt 2
<div>
                if(this.props.campsite) {
                        <div className="row"></div>
                    } else {
                        <div></div>
                    }
                    return this; 
            </div>

# renderSelectedCampsite
   renderSelectedCampsite(campsite) {
        if (campsite) {
            return (
                <Card>
                    <CardImg top src={campsite.image} alt={campsite.name} />
                    <CardBody>
                        <CardTitle>{campsite.name}</CardTitle>
                        <CardText>{campsite.description}</CardText>
                    </CardBody>
                </Card>
            );
        }
        return <div />;
    }

# sample code

    class CampsiteInfo extends Component {
    constructor(props) {
        super(props);
        this.state = {
            selectedCampsite: null
}
    } 

    checkCampsiteSelect(campsite){
        this.setState({selectedCampsite:campsite});
    }

    displayCampsite (campsite) {
        if (campsite) {
            <div className ="row" />
        }
        return <div />;
    }

    renderCampsite(campsite){
        return(
            <div className = "col-md-5 m-1">
                <Card>
                    <CardImg top src={campsite.image} alt={campsite.name} />
                    <CardBody>
                        <CardTitle>{campsite.name}</CardTitle>
                        <CardText>{campsite.description}</CardText>
                    </CardBody>
                </Card>
            </div>
        )

    }

    renderComments(){

    }
        
    render() {
        return(
            <div>
                {this.displayCampsite(this.state.campsite)}
            </div>
        );
        
    }
}

export default CampsiteInfo;

## return
   render() {
        return(
            <div>
                if (campsite) {
                    <div className ="row" />
                }
                return <div />;
            </div>
        );
        
    }

    {this.renderCampsite(this.state.campsite)}

## renderCampsite

        renderComments(comments){

        if(comments) {
            comments.map(comment => {
            return(
                    <div key={comment.id} div className = "col-md-5 m-1">
                        <h4>Comments</h4>
                        <p>{comment.text}</p>
                        <p>{comment.author}</p>
                    </div>
            )}
        }
    }