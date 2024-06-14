# Projeto-SuperCars
Modelo de página construída com base na teoria ensinada pelo canal DevClub.

Projeto todo desenvolvido em `HTML`, `CSS` e `JavaScript`, com muitas estilizações que podem ser acompanhadas logo abaixo no vídeo.
- A ideia inicial desse projeto é aprender e aplicar técnicas de estilização um pouco mais avançadas.
- As imagens foram tratadas com a IA da PicWish.
- O projeto foi criado a partir de uma ideia do canal DevClub.

https://github.com/jcamposmelo/Projeto-SuperCars/assets/101723959/c448b565-08f4-4243-a9bc-2a13791a69b5

![image](https://github.com/jcamposmelo/Projeto-SuperCars/assets/101723959/0e34c3e5-6102-48fb-a08c-19e9ee87be7d)

## 🔨 Funcionalidades do projeto

Aplicação web deste projeto permite ao usuário de forma fácil e objetiva, navegar pela página acessando os diversos carros, conforme sua intenção.

## ✔️ Técnicas e tecnologias utilizadas

As técnicas e tecnologias utilizadas foram:

- Para este trabalho, não foram utilizados `frameworks` o processo se deu de forma nativa;
- `HTML`: criação dos elementos da tela;
- `CSS`: estilização da aplicação;
- `JavaScript`: construção de elementos dinâmicos para acesso aos botões bem como a maneira de surgimento das informações utilizando a função `setSlider`.

#
## Detalhamento de trechos do código

- Esta linha de código é usada uma função para determinar em JavaScript o uso do `setSlider()`, que é utilizada para mostrar um formato de carrossel de imagens ou itens semelhantes. 
  
      function setSlider() {
       
        let itemOld = container.querySelector('.list .item.active')
        itemOld.classList.remove('active')
      
        let dotsOld = indicator.querySelector('ul li.active')
        dotsOld.classList.remove('active')
        dots[active].classList.add('active')
      
        indicator.querySelector('.number').innerHTML = '0' + (active + 1)
      }

- Estre trecho do código, controla a navegação do carrossel de imagens, permitindo mover-se para o próximo ou anterior item na lista.

      nextButton.onclick = () => {
        list.style.setProperty('--calculation', 1)
        active = active + 1 > lastPosition ? 0 : active + 1
        setSlider()
        items[active].classList.add('active')
      }
      
      prevButton.onclick = () => {
        list.style.setProperty('--calculation', -1)
        active = active - 1 < firstPosition ? lastPosition : active - 1
        setSlider()
        items[active].classList.add('active')
      }

## 📁 Acesso ao projeto

Você pode acessá-lo de forma gratuita e aprimorar!

Após baixar o projeto, você pode abrir com o Visual Studio Code. Para isso, no menu superior, clique em:

- **File** > **Open Folder**
- O projeto está salvo e pode ser acessado de forma gratuita e inclusive pode receber contribuições basta acessar por aqui mesmo. (Caso o projeto esteja compactado na extensão .zip, será necessário extraí-lo antes de procurá-lo)
- Por fim clique em OK!

Ao finalizar esses passos, você pode executar a aplicação com a extensão Live Server 🏆 


