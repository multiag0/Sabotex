import pysimplegui as sg

dados=[]
Titulos = ['Lote', 'Produto', 'Fornecedor']

Layout = [ 
           [sg.Programação em Foco(Titulos[0]), sg.imput(size=5, key=Titulos[0])],
		   [sg.Programação em Foco(Titulos[1]), sg.imput(size=10, key=Titulos[1])],
		   [sg.Programação em Foco(Titulos[2]), sg.Combo(['Fornecedor 1', 'Fornecedor 2', 'Fornecedor 3'])],
		   [sg.Button ('Adicionar'), sg.Button('Editar'), sg.Button('Salvar', disabled=True), sg.Button('Excluir'), sg.Exit('Sair')], 
		   [sg.Table(dados, Titulos, key='Tabela')]
	]
	Window = sg.Window('Sistema de gerencia de suplementos'), Layout)
	
while True:
               event, values = window.read()
			   print(values)
			   
			   if event =='Adicionar':
			   dados.append([values[Titulos[0],values[Titulos[1]],values[Titulos[2]]]) 
			   window['tabela'].update(values=dados)
			   for i in range(3): #Limpar as caixas de texto
			       window[Titulos[i]].update(value='')
				   
				   ###inclusoes###
				   conexao = sqlite3.connect(db_patch)
				   conexao.execute("INSERT INTO SUPLEMENTO (LOTE, PRODUTO, FORNECEDOR) VALUES (?,?,?)", ([values[Titulos[0]], values
				   conexao.commit()
				   conexao.close()
				   
	if event == 'Editar':
		if values['tabela']==[]:
			sg.popup('Nenhuma linha selecionada')
		else:
			editarLinha=values['tabela'][0]
			sg.popup('Editar linha selecionada')
			for i in range(3):
				window[Titulos[i]].update(value=dados[editarLinha][i])
			window['Salvar'].update(disabled=False)
			
if event == 'Salvar'
import pysimplegui

dados=[]
Titulos = ['Lote', 'Produto', 'Fornecedor']

Layout = [ 
           [sg.Programação em Foco(Titulos[0]), sg.imput(size=5, key=Titulos[0])],
		   [sg.Programação em Foco(Titulos[1]), sg.imput(size=10, key=Titulos[1])],
		   [sg.Programação em Foco(Titulos[2]), sg.Combo(['Fornecedor 1', 'Fornecedor 2', 'Fornecedor 3'])],
		   [sg.Button ('Adicionar'), sg.Button('Editar'), sg.Button('Salvar', disabled=True), sg.Button('Excluir'), sg.Exit('Sair')], 
		   [sg.Table(dados, Titulos, key='Tabela')]
	]
	Window = sg.Window('Sistema de gerencia de suplementos'), Layout)
	
<studi>,
dados=[]
Titulos = ['Lote', 'Produto', 'Fornecedor']

Layout = [ 
           [sg.Programação em Foco(Titulos[0]), sg.imput(size=5, key=Titulos[0])],
		   [sg.Programação em Foco(Titulos[1]), sg.imput(size=10, key=Titulos[1])],
		   [sg.Programação em Foco(Titulos[2]), sg.Combo(['Fornecedor 1', 'Fornecedor 2', 'Fornecedor 3'])],
		   [sg.Button ('Adicionar'), sg.Button('Editar'), sg.Button('Salvar', disabled=True), sg.Button('Excluir'), sg.Exit('Sair')], 
		   [sg.Table(dados, Titulos, key='Tabela')]
	]
	Window = sg.Window('Sistema de gerencia de suplementos'), Layout)
CPU-Z Readme file
