
import VanillaTilt from 'vanilla-tilt'


.........


constructor(props) {
    super(props)
    this.tiltRef = React.createRef();
    this.tiltLogoRef = React.createRef();
}

componentDidMount() {
    const vanillaTiltOptions = {
        max: 25,
        speed: 400,
        glare: true,
        'max-glare': 0.5,
    }
    VanillaTilt.init(this.tiltLogoRef.current, vanillaTiltOptions);
}



........... 


<div className="col-md-0">
    <div ref={this.tiltLogoRef} className="tilt-root" style={{ height: '80px', width: '100px', padding: '0', marginLeft: '10px' }}>    
        <div className="tilt-child" style={{ height: '80px', width: '100px', padding: '0', margin: '0px' }}>
            <img src={require('../../assets/images/logo.gif')} style={{ height: '80px', width: '100px', padding: '0', marginRight: '10px' }} />        
        </div>
    </div> 
</div>