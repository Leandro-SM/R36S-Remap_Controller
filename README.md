# R36S-Remap_Controller
Recuperar controles desconfigurados.

---

### Recentemente, acabei desconfigurando os botões do meu R36S e não conseguia retornar ao menu. Para corrigir, é preciso editar os arquivos na pasta emulationstation.

O arquivo pode estar:

- corrompido
- incompleto
- com XML inválido
- Teclas incorretas

Apesar da pasta autoconfigs e do retroarch/retroarchcustom.cfg em Retroarch, o arquivo que manda nos botões fica em:

    SHARE/system/configs/emulationstation/

O arquivo que você deve editar é:  

    es_input.cfg

Primeiro, copie o arquivo para outro lugar, ou crie uma cópia e renomeie para es_input.cfg.bkp.

Então você pode deletar o arquivo es_input.cfg para que o R36S retorne para o padrão

---


Teste no console.

---


Se não funcionar, abra o arquivo es_input.cfg e edite os inputs de acordo com o padrão:

    <?xml version="1.0"?>
    <inputList>
        <inputConfig type="joystick" deviceName="sunxi-joypad" deviceGUID="19000000000000000100000000010000">
            <input name="a" type="button" id="0" value="1"/>
            <input name="b" type="button" id="1" value="1"/>
            <input name="x" type="button" id="2" value="1"/>
            <input name="y" type="button" id="3" value="1"/>
    
            <input name="start" type="button" id="6" value="1"/>
            <input name="select" type="button" id="7" value="1"/>
            <input name="hotkey" type="button" id="8" value="1"/>
    
            <input name="up" type="button" id="9" value="1"/>
            <input name="down" type="button" id="10" value="1"/>
            <input name="left" type="button" id="11" value="1"/>
            <input name="right" type="button" id="12" value="1"/>
    
            <input name="leftshoulder" type="button" id="4" value="1"/>
            <input name="rightshoulder" type="button" id="5" value="1"/>
        </inputConfig>
    </inputList>


---
