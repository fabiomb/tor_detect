<?php

function IsTorExitPoint(){
    if (gethostbyname(ReverseIPOctets($_SERVER['REMOTE_ADDR']).".".$_SERVER['SERVER_PORT'].".".ReverseIPOctets($_SERVER['SERVER_ADDR']).".ip-port.exitlist.torproject.org")=="127.0.0.2") {
        return true;
    } else {
       return false;
    } 
}

function ReverseIPOctets($inputip){
    $ipoc = explode(".",$inputip);
    return $ipoc[3].".".$ipoc[2].".".$ipoc[1].".".$ipoc[0];
}
