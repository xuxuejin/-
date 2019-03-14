## vscode

  1.在使用vscode编写vue组件的时候，为了使用tab键快速生成标签，使用less编写样式不报错，需要设置一下vscode
    解决：
    "files.associations": {
        "*.vue": "vue"
    }
    
  2.vscode在使用tab键补全代码时，效果不理想，是因为vscode自带的提示功能和Emmet语法的键位冲突所导致的，自带的智能提示优先级要高于Emmet语法，所以才出现提示不灵的情况
  解决：
  首选项 --> 设置 --> 查找 emmet "emmet.triggerExpansionOnTab": false,  改为 true
