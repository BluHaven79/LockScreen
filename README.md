.App {

  text-align: center;

}



.App-logo {

  animation: App-logo-spin infinite 20s linear;

  height: 80px;

}



.App-header {

  background-color: #222;

  height: 150px;

  padding: 20px;

  color: white;

}



.App-intro {

  font-size: large;

}



@keyframes App-logo-spin {

  from { transform: rotate(0deg); }

  to { transform: rotate(360deg); }

}

import React, { PropTypes } from "react";
import ClockDisplay from "./ClockDisplay";
import TopOverylay from "./TopOverlay";
import SlideToUnlock from "./SlideToUnlock";

export default class LockScreen extend React.Component {
    static propTypes= {
    wallpaperPath: PropTypes.string,
    userInfomessage: PropTypes.string,
    onUnlocked: PropTypes.func,
    };
    
  render()
    const {
    wallpaperPath,
    userInfomessage,
    onUnlocked,
    } = this.props;
    
    return (
      <div 
      style={{
        hieght: "100%",
        display: "flex",
        justifyContent: "space-between",
        flexDirection: "column",
        backgroundImage: wallpaperPath ? 'url(${wallpaperPath})' : "",
        backgroundColor: "Black",
        backgroundPosition: "Center",
        backgroundSize: "Cover",
        }}
        
        
    
    

