# Lista Linear

Faça um fork deste repositorio e implemente a função excluirElemento

**excluirElemento:**
* Pede para o usuario digitar um numero
* Busca o numero na lista
* Se encontrado exclue o elemento e atualiza a quantidade de elementos na lista
* Se não econtrado exibe "elemento não encontrado" 

void excluirElemento()
{
	int numero;
	cout << "Digite o numero a ser excluido na lista: " << endl;
	cin >> numero;
	int pos = posicaoElemento(numero);
	if (pos != -1) {
		for (int i = pos; i < nElementos - 1; i++)
		{
			lista[i] = lista[i + 1];
		}
		nElementos--;
		cout << "O elemento foi excluido" << endl;
	}
	else
	{
		cout << "O elemento digitado nao foi encontrado" << endl;
	}
}
