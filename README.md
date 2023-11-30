# TEST-RESULTS
Zapažanja Calculator kod-a


1. У коду нема провера за делење са нулом. Код треба бити ажуриран тако да се посебно проверава делење са нулом, а померање израза треба вратити као "ERROR" у таквим случајевима.
2. Код не обрађује случајеве када су уноси невалидни. На пример, израз "1++2" или "3*+4" може представљати проблем. Требало би додати провере и обраду грешака за неисправне изразе.
3. Static променљива finalResult: Употреба static променљиве finalResult може довести до проблема.Требало би размислити о промени ове променљиве, можда коришћењем локалних променљивих у методама где је могуће.
4. Назив метода ToString() би требало да буде промењен у toString() да би се следило конвенцијама језика Java.
5.  Постоје боље начине за конверзију и поређење карактера у Java, на пример, коришћењем Character.toString(Operations.ADDITION_SYMBOL) уместо String.valueOf(Operations.ADDITION_SYMBOL).
6. За добијање израза од корисника, можда би било боље користити java.util.Scanner уместо прослеђивања израза као параметар методу Run().
7. Уместо коришћења catch (Exception exc) за хватање свих изузетака, боље би било спецификовати који изузетаке очекујете. На пример, NumberFormatException када се изврши Float.parseFloat().
8. Услови у методи evaluateExpression се могу упростити. Нпр. коришћењем метода startsWith за проверу почетка израза.
