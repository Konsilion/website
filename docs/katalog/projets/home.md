---
title: Catalogue Projets
katalog: true
hide:
    - toc
---

<div id="DatamiMain"></div>


<div id="DatamiExternal" style="display: none"></div>


<style>
    .md-button{margin: 0 10px 10px 0;}
    
    #FullDatamiExternal, #MinimizeDatamiExternal {
        float: right;
    }
    #HideDatamiExternal {
        float: right;
        background-color: #bd0000;
        color: white;
    }
    
    #DatamiExternal {
        height: 55vh;
        width: 100%; 
        overflow-y: scroll; 
        overflow-x: hidden;
        border-top: 1px solid #ddd;
        border-bottom: 1px solid #ddd;
        margin-top: 25px;
        padding: 25px;
        transition: box-shadow 0.5s, background 0.5s;
    }
    #DatamiExternal:hover {
        box-shadow: inset -3px 5px 3px #DDD,
                    inset -3px -5px 3px #DDD;
    }    
</style>

<style>
/* width */
::-webkit-scrollbar {
  width: 15px;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px #DDD; 
  border-radius: 10px;
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: #666; 
  border-radius: 10px;
  transition: background 0.5s;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: var(--md-accent-fg-color); 
}
</style>

<script>
    function ShowDatamiExternal(){    
        document.getElementById("DatamiExternal").style.display="block";
        document.getElementById("HideDatamiExternal").style.display="block";
        document.getElementById("FullDatamiExternal").style.display="block";
    }
    function HideDatamiExternal(){    
        document.getElementById("DatamiExternal").style.display="none";
        document.getElementById("HideDatamiExternal").style.display="none";
        document.getElementById("MinimizeDatamiExternal").style.display="none";
        document.getElementById("FullDatamiExternal").style.display="none"; 
        document.getElementById("DatamiExternal").style.height="55vh";
    }    
    function FullDatamiExternal(){
        document.getElementById("MinimizeDatamiExternal").style.display="block";
        document.getElementById("FullDatamiExternal").style.display="none";
        document.getElementById("DatamiExternal").style.height="auto";
    }
    function MinimizeDatamiExternal(){
        document.getElementById("MinimizeDatamiExternal").style.display="none";
        document.getElementById("FullDatamiExternal").style.display="block";
        document.getElementById("DatamiExternal").style.height="55vh";
    }       
</script>