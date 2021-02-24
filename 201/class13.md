USING HTML5 STORAGE

HTML5 Storage is based on named key/value pairs. You store information based on a named key, then you able to retrieve that information with the same key. The named key is a string. The information able to be any type supported by JS, inclusive strings, Booleans, integers, or floats. However, the information is actually stored as a string. If you are storing and retrieving anything other than strings, you will have to use functions like parseInt() or parseFloat() to coerce your retrieved information into the expected JS informationtype.

interface Storage {

getter any getItem(in DOMString key);

setter creator void setItem(in DOMString key, in any information);

};

Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception

var foo = localStorage.getItem(&quot;bar&quot;);

// ...

localStorage.setItem(&quot;bar&quot;, foo);

…could be rewritten to use square bracket syntax instead:

var foo = localStorage[&quot;bar&quot;];

// ...

localStorage[&quot;bar&quot;] = foo;

we make the localStorage object to save whether there is a game in forword (gGameInforword, a Boolean). If so, it iterates through the pieces (gPieces, a JS Array) and saves the row and column NUM of each piece. Then it saves some additional game state, inclusive which piece is selected (gSelectedPieceIndex, an integer), whether the piece is in the middle of a potential long series of hops (gSelectedPieceHasMoved, a Boolean), and the whole NUM of moves made so far (gMoveCount, an integer).