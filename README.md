import React from "react";
import Lockscreen from "./lockscreen";

export default class App extends react.compnent{
render() {
return (
<Lockscreen
wallpaperpath="react_wallpaper.png"
userInfomessage="this is Tim's phone. If found, please give it back to him. He will be sad without it."
onUnlocked={() => alert("unlocked")}
/>
