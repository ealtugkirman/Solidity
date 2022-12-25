Solidity dilinde, bir Smart Contract içinde sürekli olarak saklanan ve erişilebilir olan değişkenlere "state variable" denir. State variables, bir Smart Contract'ın depolama alanında saklanır ve bu nedenle, Smart Contract'ın çalışması bittiğinde de hala mevcut olurlar. State variables, bir Smart Contract içindeki fonksiyonlar arasında paylaşılır ve bu nedenle, bir Smart Contract'ın işlevleri arasında birbirleriyle iletişim kurabilirler.

State variables, Solidity dilinde "public" veya "private" olarak tanımlanabilir. "Public" olarak tanımlanan state variables, dışarıdan da erişilebilir hale getirilir ve bu nedenle, dışarıdan bir fonksiyon veya başka bir Smart Contract tarafından da okunabilir ve değiştirilebilir olurlar. "Private" olarak tanımlanan state variables ise, sadece Smart Contract içindeki fonksiyonlar tarafından okunabilir ve değiştirilebilir olurlar.

Örneğin, aşağıdaki örnekte, "balance" adında bir "public" state variable tanımlanmıştır:


pragma solidity ^0.6.0;

contract ExampleContract {
  uint public balance;

  function setBalance(uint _balance) public {
    balance = _balance;
  }
}
Bu örnekte, "balance" state variable'ı, "setBalance" fonksiyonu tarafından değiştirilebilir ve dışarıdan da okunabilir hale getirilmiştir. Bu state variable, bir Smart Contract'ın depolama alanında saklanır ve bu nedenle, Smart Contract'ın çalışması bittiğinde de hala mevcut olur.
