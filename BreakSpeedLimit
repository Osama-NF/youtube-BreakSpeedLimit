document.getElementById('player-theater-container').addEventListener("keydown", e => {
    if (event.key === '+' || event.key === '-' || event.key === 'z' || event.key === 'x') {
        if (document.getElementById('currentSpeedDivMadeByONF')) document.getElementById('currentSpeedDivMadeByONF').remove();
        if (event.key === "+" || event.key === 'x') document.getElementsByTagName("video")[0].playbackRate += 0.25;
        else if (event.key === "-" || event.key === 'z') document.getElementsByTagName("video")[0].playbackRate -= 0.25;

        let currSpeed = document.createElement('div');
        currSpeed.id = 'currentSpeedDivMadeByONF';
        currSpeed.textContent = 'Custom Speed: ' + document.getElementsByTagName("video")[0].playbackRate;
        currSpeed.style.cssText = 'background: rgba(0,0,0,0.4); color: white; position: absolute; top: 20%; left: 45%; font-size: 23px; padding:5px; user-select: none;';

        
        document.getElementById('player-theater-container').append(currSpeed)
        setTimeout(() => currSpeed.remove(), 500)
    }
})
