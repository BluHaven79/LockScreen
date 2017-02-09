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
        
        
    
    

