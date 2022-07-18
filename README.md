# automa-odebackup
automação para backup em google drive


import pyautogui
import time

#abrir arquivo e google chrome para automação de backup

#exibe alerta antes de iniciar automação
pyautogui.alert('Iniciando atualização, click em OK para continuar e aguarde a conclusão!')
#tempo de execução de cada codigo
pyautogui.PAUSE = 0.5
#press para apertar botão de teclado
pyautogui.press('winleft')
#pesquisa o programa selecionado
pyautogui.write('chrome')
#abre programa selecionado
pyautogui.press('enter')

#dar tempo para abertura de programa
time.sleep(1)
#imprimi link ou local de arquivos
pyautogui.write('https://drive.google.com/drive/u/0/my-drive')
#enter para iniciar rodagem 
pyautogui.press('enter')
#atalho para abrir area de trabalho
pyautogui.hotkey('winleft','d')
#posição do mouse, definir posição do mouse (eixos x,y)
#mover mouse, definir posição
pyautogui.moveTo()
#pressiona botão do mouse e mantém pressionado
pyautogui.mouseDown()

#posiciona onde quer soltar arquivos (definir eixos)
pyautogui.moveTo()

#alterar tela dentro do movimento

pyautogui.hotkey('alt', 'tab')

time.sleep(1)
#soltar o botão do mouse
pyautogui.mouseUp()

time.sleep(6)

pyautogui.alert('Computador liberado para utilização')
