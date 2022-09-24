# wordpress
Modified wordpress code, adapted to optimization on litespeed server.

W pliku konfiguracyjnym (wp-config.php) znajduje się sekcja z kluczami. Wykorzystywane są one do autoryzacji oraz enkrypcji, dlatego warto zadbać o to, aby każda instancja WordPressa, posiadała unikalne klucze. Wykorzystywanie tych samych kluczy, na wielu stronach, jest niebezpieczne.

Niektóre autoinstalatory, używają tych samych kluczy dla każdego zainstalowanego WordPressa. Przykładowa sekcja z kluczami wygląda tak: 

define('AUTH_KEY',         'q*jp ]9+m+!*a./uTdi+sA8B,zu&9uG#I3<P>~^+9Y1)8JE(!rR^HzL:zCDNpfRq');
define('SECURE_AUTH_KEY',  ',/~Bk;-$)B{UO=Hw!xE>U^NVS|)!!8T9lG=YS}r!%]2/4Y1A! TF]cX8`fZ1_}$u');
define('LOGGED_IN_KEY',    ';;q-<GC#pUzDL)w?C14mL5,]D4U=2{$}f/nxvaB_UgO++l+T=:W[p^Z*&|a)M7%l');
define('NONCE_KEY',        'YwIqTF.9Uored=(2.OdFO_w(W-dX6/.A#9J=?:VMs|/g$MB4@~pIVfAfjJGpO9og');
define('AUTH_SALT',        'tNyV4f8@F/0u!Nc]s:M/x880L.Lq# o0-rt+Q#mgcsF9~Jd!yXcQm9xjWto-wjIL');
define('SECURE_AUTH_SALT', 'Z1#>vdmkEF-N:XV=J-P|~m(|EP|E+ltu)-37k]33M>jjK5gVX@Vm qiCKvZ($@J6');
define('LOGGED_IN_SALT',   'S}e9&PrS:8j,H/C9`#3k*qORpb?gAgJ;jDZNeXL=19L/X&uBMXQ1o*Tb+<n0j3,b');
define('NONCE_SALT',       'K=^Bz._`K{9]Pe ?xk0(rsgExR<xHu$XNOS8:@zr&kxvy+S[qcm<HOoZeS-JG70=');

Generator kluczy dostępny jest pod linkiem: https://api.wordpress.org/secret-key/1.1/salt/
