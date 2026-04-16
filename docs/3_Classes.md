**Aluno** - RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
  contratarPlano()
	agendarAula()
	cancelarAgendamento()
	atualizarStatus()
	registrarAcesso()
	receberNotificacao()

**Plano** - RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
  criarPlano()
	editarPlano()

**Pagamento** - RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
  registrarPagamento()
	confirmarPagamento()
	cancelarPagamento()

**Acesso** - RF05, RF09
- idAcesso
- dataHora
- autorizado
  registrar()
	autorizar()
	negar()

**Aula** - RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima
  disponiblizarHorario()
	reservarVaga()
	liberarVaga()
	registrarPresenca()

**Agendamento** - RF06, RF10
- idAgendamento
- dataReserva
- status
  confirmar()
	cancelar()

**Presenca** - RF07
- idPresenca
- data
- presente
  registrar()
	consultar()

**AvaliacaoFisica** - RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
  registrar()
	atualizarDados()
	anexarArquivo()

**Notificacao** - RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
  enviar()
	marcarComoLida()

**Instrutor** - RF07, RF08
- idInstrutor
- nome
- especialidade
  realizarAvaliacaoFisica()
	registrarPresenca()

**Recepcionista** - RF01, RF03
- idRecepcionista
- nome
  cadastrarAluno()
	registrarPagamento()

**Gerente** - RF02, RF09
- idGerente
- nome
  gerenciarPlanos()
	emitirRelatorios()
