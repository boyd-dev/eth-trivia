## 이더리움 토막상식(3-1)

1. Lido의 점유율 문제  
이더리움의 지분증명 프로토콜은 위임(delegation)이 없다. 자신이 소유한 32개의 이더를 예치하고 직접 노드를 운영해야 한다. 또 그렇게 예치된 이더는 검증자 자격을 반납하고 모두 인출하기 전까지는 락업 상태에 있다.  
하지만 32개 미만의 이더를 가진 사람들도 지분증명에 참여할 수 있는 방법이 생겨났고 이것을 통칭하여 "스테이킹 풀(pool)" 서비스라고 한다. 수량에 상관없이 여러 사람들로부터 이더를 모아서 노드를 운영할 수 있는 것이다. 물론 작업증명 시대에도 마이닝 풀이라는 것이 있었으므로 지분증명도 그와 유사한 서비스가 생겨날 것이라는 것은 충분히 예상할 수 있는 일이다.  
더구나 이런 서비스들은 검증 노드를 대신 운영해주는 것을 넘어 락업된 이더를 유동화시킨 토큰을 발행하여 지급한다. 이런 형태를 "Liquid Staking (Derivatives 또는 Token)"이라고 한다. 이렇게 발행된 토큰은 원칙적으로 예치된 이더와 1:1의 가치를 지니면서 자유롭게 유통될 수 있다.  
대표적인 Liquid Staking 서비스 중 하나가 바로 [Lido](https://lido.fi/)이다. 사용자가 이더를 예치하면 다른 사람들의 이더와 함께 최소 수량 32개를 채워서 다수의 "Operator"에게 배분한다. 실제 노드를 운영하는 사람은 Lido에 등록한 Operator가 되고 그에 따른 검증 보상이 각 사용자별로(수수료 제외) 적립된다.  
Lido는 나중에 이더로 환매할 수 있는 "유동화" 토큰인 "stETH"를 발행하여 사용자에게 준다. 
새로 발행된 stETH는 다양한 디파이 서비스의 ETH/stETH 풀에서 이더와 스왑하거나 재예치 할 수 있으므로 그냥 락업되는 것보다 유리한 점이 있다. 이더와 1:1이지만 거래소나 풀에서는 보통 조금 할인된 가격으로 거래된다.  

   Lido는 형식적으로 DAO이며 거버넌스 토큰인 LDO 홀더들의 투표로 주요한 정책이 결정된다. 그러나 대부분 거버넌스 토큰 분배가 소수의 투자자와 설립자들, 이해관계자들에게 집중되어 있는 것처럼 Lido는 중앙화된 주체에 의해 움직이고 이더리움의 원래 설계 사상과는 무관한 방향으로 흘러갈 수 있다. 이더리움 재단의 Danny Ryan은 자신의 블로그에 "[The Risks of LSD](https://notes.ethereum.org/@djrtwo/risks-of-lsd)"이라는 글로 이에 대한 문제를 제기하기도 했다.  
   
   이러한 리스크는 최근 Lido에 속한 검증 노드가 전체의 [33% 가까이 차지하면서](https://twitter.com/lidodominance/status/1707757122291646495) 더 커지고 있다. 심지어 이더리움 거버넌스가 사실상 Lido가 될 것이라고 예측하는 하는 사람들도 있다.  

   stETH는 이론적으로는 이더와 1:1로 교환할 수 있지만 암호화폐의 특성상 가격이 불안정하기 때문에 stETH의 존재 자체가 부정적인 영향을 주기도 한다. 암호화폐 대부업체들의 무분별한 고금리 정책으로 stETH 발행과 재예치가 늘어났고 2022년 하반기 테라, 알라메다, 셀시우스, FTX 등의 파산이 이어지면서 stETH를 담보로 하거나 연계되어 있는 대출 상품들이 부실화되기 시작했다. 이더와 stETH의 가격이 "디페깅"되면서 stETH를 이더로 바꾸려는 "뱅크런"도 발생했다. 이성적으로는 이더와 1:1로 바꿀 수 있는 stETH를 할인된 가격으로 매수할 수 있는 기회일 수도 있었겠지만 반대로 생각하면 stETH가 이더와 동일하고 아직 비콘체인에서 인출이 불가능하다면 이더리움 자체도 위험할 수 있다는 인식이 확산되면서 이더 가격의 폭락으로 이어지게 되었다(2022년 8월 2000달러에서 11월 1200달러 아래까지 하락).  

   Lido가 이더리움 지분증명에 기여하는 바가 없지는 않지만 소수의 지분 비율이 계속 늘어나고(Lido에서 노드를 운영하는 주체는 대략 30개 미만) 또 stETH의 발행으로 인한 여러 파생 상품들의 잠재된 위험은 이더리움 생태계의 건전성과는 무관한 것이 사실이다. 이더리움에서는 Lido가 자체적으로 스테이킹 비율의 상한을 33% 미만으로 강제해야 한다고 주장했지만 Lido DAO는 "self-limiting" [안건](https://snapshot.org/#/lido-snapshot.eth/proposal/0x10abedcc563b66b1adee60825e78c387105110fa4a1e7354ab57bc9cc1e675c2)에 대해 99%가 반대했다. Lido 외의 다른 스테이킹 서비스들(RocketPool, Stakewise 등)은 22% 미만으로 제한하는 것에 동의했다.  

   Lido의 입장은, 어차피 기관들이 진입하게 되면 일반 사용자들 뿐만 아니라 기관들을 대상으로 하는 스테이킹 서비스들도 나타나게 되고(Alluvial 처럼) 결국 중앙화된 주체의 지분이 임계치에 이르는 것은 시간문제라고 주장한다. Lido DAO는 그런 상황에서 상대적으로 탈중앙화된 스테이킹 서비스가 될 수 있다.  
   높은 지분 비율과 중앙화에 대한 우려는 언뜻 보면 비슷한 문제일 수도 있지만 앞으로 나타날 것으로(또는 확산될 것으로) 예상되는 중앙화된 서비스와 경쟁하기 위해서는 Lido가 지분의 한계를 두어서는 안된다는 말에도 일리가 아예 없지는 않다.  


2. 검증자 증가에 따른 문제  
지분증명은 다수의 개별 주체가 운영하는 검증 노드가 많을수록 탈중앙화와 보안성이 높아진다. 이더리움은 인출이 가능하게 된 Shapella 하드포크 이후 검증자들이 꾸준히 늘었다. 하지만 검증자 수가 계속 늘어나면 노드들 사이의 전파되는 메시지(attestation) 수도 늘어난다. 대략 노드 수가 N개 일때 O(N²)으로 증가하기 때문에 네트워크 트래픽의 과부하가 발생할 수 있다. 현재 추세대로 가면 수 개월내에 우려할만한 상황이 나올 수도 있다고 전망하는 [의견](https://www.coindesk.com/consensus-magazine/2023/09/29/the-most-pressing-issue-on-ethereum-is-validator-size-growth/)도 있다.  

   EIP-7251에서는 유효잔액을 늘려서 검증자의 과도한 증가를 억제해야 한다는 제안이 있었다. 하지만 이 제안은 유효잔액 값이 프로토콜 내에서 중요하게 사용되기 때문에 고려해야할 점들이 많이 있다. 그래서 비교적 손쉽게 적용할 수 있는 churn limit을 제한하는 EIP-7514가 진행 중으로 잠정적으로 1 epoch에 유입되는 검증자를 8개로 제한할 것을 제안했다. churn limit은 검증자 대기자 수가 늘어나면 자동으로 그에 비례하여 증가하도록 되어 있는데 현재(2023.9) 12로 계속 늘어나고 있다.  


3. 롤업 Escape Hatch  
롤업의 기본 전제는 L2의 거래 내역들의 정합성을 탈중앙화된 L1이 보장한다는 것이다. 그러나 실제 거래가 발생하는 곳은 L2이고 L1의 자산이 브리지를 통해 L2로 이전되므로 L2 자체를 어느 정도는 믿어야 한다는 현실적인 문제도 있다.  
L2의 거래를 실제 실행시켜 주는 것은 시퀀서들이다. 현재(2023.9) 모든 L2 플랫폼들은 개발팀이 시퀀서를 직접 운영하고 있기 때문에 완전히 중앙화된 서버의 형태로 움직이고 있다. (그럴 일은 거의 없겠지만) 만약 시퀀서가 중지되거나 해킹으로 문제가 발생하는 경우 L2로 이전된 자산을 다시 L1으로 옮길 수 있는 방안이 필요하다. 즉 L2가 제대로 동작하지 않더라도 강제적으로 자산을 복구할 수 있는 방법이 필요한 것이다. 이러한 방안을 통칭하여 "Escape Hatch"라고 한다. 각 L2 시스템들이 Escape Hatch를 구현하고 있는지를 알아보려면 [L2BEAT](https://l2beat.com)를 참조(평가 항목 "SEQUENCER FAILURE").  
Escape Hatch는 L2가 탈중앙화 되어 있다면 필요하지 않을 수 있다. 왜냐하면 단 하나의 정직한 시퀀서가 살아 있다면(또 충분한 컴퓨팅 리소스가 제공된다면) L2의 거래는 항상 처리될 것이기 때문이다.  


4. 전자서명과 트랜잭션  
이더리움은 ECDSA를 사용하여 트랜잭션에 "EOA" 계정(Externally Owned Account)으로 서명한다. EOA라는 이름에서 알 수 있는 것처럼 계정은 이더리움 네트워크에 연결하지 않아도 오프라인에서 만들 수 있다. 그래서 거래 메시지를 오프라인에서 서명하고 그 데이터(트랜잭션)를 나중에 이더리움에 전송할 수 있다. 서명을 위해서는 당연히 EOA 계정의 개인키가 필요하다.  
이더리움 클라이언트의 JSON-RPC가 제공하는 서명 메소드는 3가지 정도가 있다.  
    - eth_sign
    - personal_sign
    - eth_signTransaction  

   JSON-RPC는 사용 목적에 따라 네임스페이스가 정해져 있는데 앞에 붙은 `eth_`와 `personal_` 은 각각 `eth` 네임스페이스와 `personal` 네임스페이스에 속해 있다는 것을 의미한다(`personal`은 현재 deprecated). 두 메소드는 모두 일반적인 메시지를 해시한 후 EOA 계정으로 서명하는 용도이다. 임의의 데이터를 `keccak256` 해시하여 32바이트를 만든 후에 서명하므로 서명된 결과는 모두 길이가 65바이트로 같다. 서명할 때 해시 하기 전의 메시지를 표시하려면 `personal_sign`을 사용한다.  

   `eth_signTransaction`은 트랜잭션 데이터를 서명할 때 사용한다. 파라미터로 트랜잭션 객체를 전달한다.  
   ```
   {nonce, type, from, to, gasLimit, maxFeePerGas, maxPriorityFeePerGas, value, data, chainId }
   ```
   알케미와 같은 프로바이더들은 위의 RPC들을 직접 제공하지 않는 경우가 대부분이다. 왜냐하면 RPC 호출을 하지 않아도 ethers와 같은 라이브러리를 통해 얼마든지 서명을 할 수 있기 때문이다. 더구나 개인키를 파라미터로 전달해야 하는데 이것은 보안적으로 매우 위험한 일이다.  


   ethers(v5.7) 에서는 아래와 같이 `signMessage(message)`를 이용하여 서명할 수 있다.  
   ```
   const privateKey = "...";
   const provider = new ethers.providers.JsonRpcProvider("...");

   const message = "Hello, Ethereum";
   const messageHash = ethers.utils.hashMessage(message);
   console.log(messageHash);
   const wallet = new ethers.Wallet(privateKey, provider);

   wallet.signMessage(message).then(signature => {
    
   const r = signature.slice(0, 66)
   const s = '0x' + signature.slice(66, 130)
   const v = '0x' + signature.slice(130, 132)    
    
   console.log(r,s,v);
    
   }); 
   ```
   ethers는 라이브러리에서 자동으로 메시지 앞에 `\x19Ethereum Signed Message:\n`라는 prefix를 추가하여 다시 해시한다. 이것은 애플리케이션에서 사용자들에게 일반 메시지로 위장한 트랜잭션 서명을 유도하여 자금을 인출하는 경우를 막기 위해 트랜잭션과 일반 메시지의 서명을 구분하려는 목적이 있다. 서명된 메시지를 솔리디티의 `ecrecover`로 확인하려면 prefix가 있는 메시지를 해시하여 전달해야 한다.  

   ethers에서 트랜잭션 서명은 `signTransaction(transactionRequest)`을 사용한다. 보통은 애플리케이션에 지갑이 연결되어 있으므로 트랜잭션 서명 데이터를 만들 필요 없이 `signer.sendTransaction`을 사용하고 지갑에서 서명하면 트랜잭션을 전송할 수 있다. 서명된 raw 트랜잭션은 이더리움 클라이언트의 JSON-RPC 호출 `eth_sendRawTransaction`으로도 전송할 수 있다.  
   
   서명하기 전에 해시된 메시지가 표시되는 경우 사용자가 어떤 내용인지 알 수 없기 때문에 이를 보완하기 위해 [EIP-712: Typed structured data hashing and signing](https://eips.ethereum.org/EIPS/eip-712)가 채택되었다. EIP-712 예제는 [여기](https://github.com/boyd-dev/sample-sign712)를 참조  

   이더리움의 트랜잭션은 트랜잭션 객체의 RLP 인코딩과 그것을 해시한 전자서명으로 구성된다. 예를 들어 아래와 같은 트랜잭션 객체가 있다고 하면
   ```
   const tx = {
        nonce: 0x68, 
        to,
        value,
        gasLimit,
        maxFeePerGas,
        maxPriorityFeePerGas,
        'type': 2,
        'chainId': 5
   }
   ```
   이것을 다음과 같이 서명 없는 raw 트랜잭션을 만들 수 있다.
   ```
   ethers.utils.resolveProperties(tx).then((p)=> {
         const unsignedRawTx = ethers.utils.serializeTransaction(p);
         console.log(unsignedRawTx);
   }); 
   ```
   `serializeTransaction`에서 RLP 인코딩이 수행되어 `unsignedRawTx`가 만들어지고 이것을 해시한 것에 대해 전자서명 한다.
   ```
   const m = ethers.utils.keccak256(unsignedRawTx);
   const {r,s,v} = new ethers.utils.SigningKey("0x" + privateKey).signDigest(m);
   console.log(v);
   ```
   최종적으로 서명된 트랜잭션을 만들기 위해서는 서명을 포함시켜 `serializeTransaction`을 하면 된다. 
   ```
   const signedRawTx = ethers.utils.serializeTransaction(p, signature);
   ```
   여기서 `signature`는 `{r,s,v}`를 하나의 문자열로 연결한 65바이트 서명이다. `signedRawTx`을 다시 트랜잭션 객체로 복원하려면 `parseTransaction`을 사용한다.
   ```
   const tx = ethers.utils.parseTransaction("0x02f8720568843b9aca008504a817c80082520894547d73355a851079e0395adb2c647821b74c7eaf870aa87bee53800080c080a096d1c0f4a2bbc981739e2744ffc562b3c297688eb1bf901f95f3039355e8b044a054d0fb8c480e9721b4406fe64a957c5f7c79b81385aaacda1b8dd9dce342c775");
   console.log(tx);
   ```

5. EIP-1559  
이더리움은 트랜잭션을 처리하는 블록의 용량(block gas limit)이 한정되어 있기 때문에 많은 트랜잭션이 몰리는 경우에는 pending 상태가 늘어나고(며칠 동안 pending에 머물러 있는 경우도 있다) 그에 따라 가스비(수수료)는 천정부지로 높아지는 상황이 발생할 수 있다.  
EIP-1559는 2021년 8월 런던 하드포크에 적용된 "fee market" 즉 가스비 체계의 변경이다. 이것은 그동안 가스비가 수요에 따라 변동폭이 심하고, 때로는 급격하게 오르는 것을 완화하려는 목적이 있다. 근본적으로는 수요와 공급에 의해 가스비가 오르는 것을 해결할 수는 없지만 사용자가 막연하게 가스비를 추산하여 보내는 방식에서 벗어나 어느정도 예측가능한 가스비, 즉 가스비를 이 정도 내면 즉시 처리될 수 있다는 것을 알려주는 "표준 요금표"를 제공하는 것이 목적이다.  
1559에 새로 도입된 개념이 "기본 수수료(BASE FEE)"인데, 말 그대로 기본 수수료+ɑ 정도만 부담하면 트랜잭션이 다음 블록에서 항상 처리되는 것을 보장한다. ɑ를 "priority fee"라고 부른다. 이렇게 하면 이더리움 자체에서 기본 수수료가 계산되므로 사용자가 내는 전체 수수료(기본 수수료+ɑ)의 수준을 미리 파악할 수 있다는 장점이 있다. 기본 수수료의 존재는 현재 네트워크의 트랜잭션 수요를 나타내는 것으로 볼 수 있다. priority fee는 블록 생성자가 트랜잭션을 더 빨리 처리하도록 유인하는 "팁"에 해당하는 것으로 더 많은 팁을 주면 즉시 처리 가능한 것은 마찬가지다. 그래서 1559는 가스비가 저렴해지는 것과는 직접적인 관련이 없다.  

   과거에는 블록의 용량을 블록을 만드는(당시에는 채굴자) 주체가 결정했다. 하지만 1559부터는 1500만을 기준으로 트랜잭션 수요가 많으면 3000만까지 늘어날 수 있도록 했다. 1500만에 머물러 있다면 기본 수수료에 1-2gwei 만 더 내면 처리 가능하다. 하지만 블록의 사용량이 1500만을 넘는다면 다음 블록에서 기본 수수료가 오르게 된다. 반대로 1500만 미만이 되면 기본 수수료는 다시 내려간다.  
기본 수수료는 최대 인상폭이 12.5%로 상한이 정해져 있기 때문에 급격하게 오르지 않도록 되어 있다. 사용량이 1500만에서 상한인 3000으로 2배가 늘어나면 기본 수수료는 12.5%가 인상되는 셈이다. 물론 계속 상한까지 채워지면 매 블록마다 12.5%씩 증가하고 사용자들이 결정하는 ɑ도 있으므로 여전히 높은 가스비가 지속될 수는 있다.  

   1559 이전에는 모든 수수료가 블록 생성자에게 지급되었지만 이제는 기본 수수료가 소각된다. 따라서 블록 생성자에게 돌아가는 트랜잭션 처리 수수료는 ɑ에 해당하는 priority fee 뿐이다(덕분에 다른 수익원인 MEV에 대한 중요도가 높아졌다). 1559의 소각과 지분증명 전환으로 인해 신규 이더의 발행량이 실질적으로 마이너스가 되기 때문에 이더리움을 ["ultra sound money"](https://ultrasound.money)라고 말하기도 한다.  

   트랜잭션 항목에도 기존의 `gasPrice`는 의미가 없어졌고 대신 `maxFeePerGas`와 `maxPriorityFeePerGas`라는 항목이 추가되었다. `maxFeePerGas`는 사용자가 부담할 수 있는 최대 가스비이고 `maxPriorityFeePerGas`는 priority fee에 해당한다. 기본 수수료가 `maxFeePerGas`보다 작은 경우, 기본 수수료+ɑ가 `maxFeePerGas` 미만이라면 기본 수수료+`maxPriorityFeePerGas`만을 내면 된다. 기본 수수료+ɑ가 `maxFeePerGas`이상이면 `maxFeePerGas`만 부담한다. 그러나 기본 수수료 자체가 `maxFeePerGas`보다 크면 `maxFeePerGas` 아래도 떨어질 때까지 pending 상태로 머물러 있게 된다. 따라서 사용자는 자신의 트랜잭션이 pending 되는 것을 선택하거나 아니면 나중에 보낼 것인지 판단할 수 있는 여지가 생긴다.  

   다음 블록의 기본 수수료는 현재 블록에서 계산될 수 있다. 또 `eth_gasPrice` 대신에 `eth_feeHistory` JSON-RPC를 사용하면 적절한 priority fee를 결정할 수 있는 데이터를 얻을 수 있다.  


6. 

[Home](../README.md)