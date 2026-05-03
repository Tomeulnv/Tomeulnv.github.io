---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '4rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: "I'm a 3rd year PhD student in Statistics at the [University of Bologna](https://www.unibo.it/en), supervised by [Pietro Biroli](https://sites.google.com/site/pietrobiroli/) and [Elisabetta De Cao](http://elisabettadecao.com/). I'm funded by the Marie Skłodowska-Curie Actions as part of the European Social Science Genetics Network ([ESSGN](https://essgn.org/)) project.\n\nMy research mainly focuses on how educational policy and genetics interact to shape inequality in outcomes such as education, wages, family formation, and health."
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf?v=20260503
      headings:
        about: 'About'
        education: ''
        interests: 'Research Interests'
    design:
      date_format: 'January 2006'
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: false

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #       I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.

  #       Please reach out to collaborate 😃
  #   design:
  #     columns: '1'

  - block: markdown
    id: tic-tac-toe
    content:
      title: '🎮 Break Time'
      text: |-
        Surprised you scrolled this far... Fancy a quick game?
        <div id="ttt-game" style="text-align:center;">
          <p id="ttt-status" style="font-size:1.1rem;font-weight:600;margin-bottom:.6rem;">Your turn (X)</p>
          <div id="ttt-board" style="display:inline-grid;grid-template-columns:repeat(3,64px);gap:4px;"></div>
          <br>
          <button id="ttt-reset" style="margin-top:.8rem;padding:.35rem .9rem;border:1px solid rgba(0,0,0,.18);border-radius:999px;background:transparent;font-size:.88rem;font-weight:600;cursor:pointer;">Reset</button>
        </div>
        <script>
        (function(){
          var board,turn,over;
          var wins=[[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]];
          var el=document.getElementById('ttt-board');
          var st=document.getElementById('ttt-status');
          var borderC='#1f2937';
          var bgC='#374151';
          var hoverC='#4b5563';
          var txtC='#f9fafb';
          function cellStyle(){return 'width:64px;height:64px;font-size:1.6rem;font-weight:700;border:2px solid '+borderC+';border-radius:6px;background:'+bgC+';cursor:pointer;color:'+txtC+';';}
          function emptyCells(){
            var out=[];
            for(var i=0;i<board.length;i++) if(!board[i]) out.push(i);
            return out;
          }
          function findWinningMove(mark){
            for(var i=0;i<wins.length;i++){
              var w=wins[i];
              var a=board[w[0]],b=board[w[1]],c=board[w[2]];
              if(a===mark&&b===mark&&!c) return w[2];
              if(a===mark&&c===mark&&!b) return w[1];
              if(b===mark&&c===mark&&!a) return w[0];
            }
            return -1;
          }
          function bestCpuMove(){
            var winMove=findWinningMove('O');
            if(winMove>=0) return winMove;
            var blockMove=findWinningMove('X');
            if(blockMove>=0) return blockMove;
            if(!board[4]) return 4;
            var corners=[0,2,6,8].filter(function(i){return !board[i];});
            if(corners.length) return corners[Math.floor(Math.random()*corners.length)];
            var rest=emptyCells();
            return rest[Math.floor(Math.random()*rest.length)];
          }
          function renderMove(i,mark){
            board[i]=mark;
            var b=el.children[i];
            b.textContent=mark;
            b.disabled=true;
            b.style.cursor='default';
          }
          function init(){
            board=Array(9).fill('');turn='X';over=false;
            el.innerHTML='';st.textContent='Your turn (X)';
            for(var i=0;i<9;i++){
              var b=document.createElement('button');
              b.setAttribute('style',cellStyle());
              b.dataset.i=i;
              b.addEventListener('click',play);
              b.addEventListener('mouseenter',function(){this.style.background=hoverC;});
              b.addEventListener('mouseleave',function(){this.style.background=bgC;});
              el.appendChild(b);
            }
          }
          function check(m){
            for(var i=0;i<wins.length;i++){
              var w=wins[i];
              if(board[w[0]]===m&&board[w[1]]===m&&board[w[2]]===m) return true;
            }
            return false;
          }
          function play(e){
            if(over||turn!=='X') return;
            var i=+e.target.dataset.i;
            if(board[i]) return;
            renderMove(i,'X');
            if(check('X')){st.textContent='You win!';over=true;return;}
            if(board.every(function(c){return c;})){st.textContent="It's a draw!";over=true;return;}
            turn='O';
            st.textContent='Thinking...';
            setTimeout(function(){
              if(over) return;
              var cpuMove=bestCpuMove();
              renderMove(cpuMove,'O');
              if(check('O')){st.textContent='I win!';over=true;return;}
              if(board.every(function(c){return c;})){st.textContent="It's a draw!";over=true;return;}
              turn='X';
              st.textContent='Your turn (X)';
            },220);
          }
          document.getElementById('ttt-reset').addEventListener('click',init);
          init();
        })();
        </script>
    design:
      columns: '1'
      spacing:
        padding: [6rem, 0, 2rem, 0]

  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publications
  #       featured_only: true
  #   design:
  #     view: article-grid
  #     columns: 2
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ''
  #     filters:
  #       folders:
  #         - publications
  #       exclude_featured: false
  #   design:
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - events
  #   design:
  #     view: card
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: blog
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 10
  #     # Filter on criteria
  #     filters:
  #       author: ''
  #       category: ''
  #       tag: ''
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ''
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: card
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
