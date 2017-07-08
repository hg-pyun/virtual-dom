# virtual-dom
Virtual DOM에 관해 공부한 내용과 직접 만들어 보면서 기록한 repository 입니다.  
The repository is that I study about Virtual DOM and record it by myself.

## Theory
Virtual DOM에 대한 아티클은 다음을 참고하도록 하자.
- [Why? Virtual DOM EN](https://hashnode.com/post/the-one-thing-that-no-one-properly-explains-about-react-why-virtual-dom-cisczhfj41bmssp53mvfwmgrq)
- [Wyh? Virtual DOM KR - Veloper](https://velopert.com/3236)

## Structure
Virtual DOM은 크게 세부분으로 나눌수 있다.
- create : Virtual DOM에서 사용하는 가상 트리와 Node를 만드는 작업.
- diff : 이전 트리(prevTree)와 새로운 트리(newTree)를 비교하여 차이점(patches)을 반환하는 작업.
- patch : root노드에 차이점(patches)를 반영하는 작업.

#### Create
Virtual DOM Node를 만든다.
- createVNode(tagName, properties, children)
- render

#### diff
이전 노드와 현재노드를 비교하여 patches를 return 한다.
patch에는 여러타입이 존재한다.

#### patch
루트노드와 patches를 전달하여 Real DOM을 업데이트 한다.

## Reference
- [Virtual-DOM](https://github.com/Matt-Esch/virtual-dom)
- [Simple-Virtual-DOM](https://github.com/livoras/simple-virtual-dom)