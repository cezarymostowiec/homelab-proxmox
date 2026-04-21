# homelab-k8s

Mój homelab Kubernetes na Proxmox.

## Aktualny stack

- Ubuntu 24.04
- Kubernetes 1.35.x (kubeadm)
- containerd
- Calico
- MetalLB
- ingress-nginx
- cert-manager

## Struktura

- `infra/` – komponenty infrastrukturalne klastra
- `apps/` – aplikacje wdrażane do klastra

## Infra

### Calico
Konfiguracja CNI dla klastra.

### MetalLB
Pula adresów dla usług typu LoadBalancer.

### ingress-nginx
Kontroler ingress wystawiony przez MetalLB.

### cert-manager
Zarządzanie certyfikatami TLS.

## Uwagi

To repo nie powinno zawierać:
- kubeconfigów
- sekretów
- prywatnych kluczy
- wygenerowanych certyfikatów
