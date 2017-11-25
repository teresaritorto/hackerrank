process.stdin.resume();
process.stdin.setEncoding('ascii');

var input_stdin = "";
var input_stdin_array = "";
var input_currentline = 0;

process.stdin.on('data', function (data) {
    input_stdin += data;
});

process.stdin.on('end', function () {
    input_stdin_array = input_stdin.split("\n");
    main();    
});

function readLine() {
    return input_stdin_array[input_currentline++];
}

/////////////// ignore above this line ////////////////////

//solution
function main() {
    const s = readLine();
    const t = readLine();
    const k = parseInt(readLine());

    return canTransformWithinLimit(s, t, k) ? console.log('Yes') : console.log('No');
}

function canTransformWithinLimit(s, t, k) {
    if (s === t) {
        return true;
    }
    
    if (k >= s.length + t.length) {
        return true;
    }
    
    const minimumOperations = getMinimumOperations(s, t, k);
    
    if (k < minimumOperations) {
        return false;
    }
    
    return((( k - minimumOperations) & 1) == 1) ? false : true;
}

function getMinimumOperations(s, t, k) {
     let idx = s.length - 1;
    
     for(var i = 0; i < s.length; i++) {
        if ( (i >= t.length) || (s.charAt(i) != t.charAt(i)) ) {
            idx = i;
            break;
        }
    }
    
    return (s.length - idx) + (t.length - idx);
}
