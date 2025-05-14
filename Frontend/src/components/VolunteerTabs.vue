<script setup>
// Importa el archivo base de estilos CSS
import '../assets/base.css'

// Importa los componentes necesarios desde la UI personalizada del proyecto
import { Tabs, TabsContent, TabsList, TabsTrigger } from '@/components/ui/tabs'
</script>

<template>
    <!-- Contenedor principal con diseño flexible en fila y fondo gris claro -->
    <div class="flex flex-row justify-center align-middle bg-gray-50 border-b border-gray-200">
        <!-- Componente Tabs con valor por defecto "account" (no usado en este fragmento, pero puede ser útil si se agregan contenidos) -->
        <Tabs default-value="account">
            <!-- Lista de pestañas -->
            <TabsList>
                <!-- Pestaña para Emergencias Activas -->
                <TabsTrigger value="emergencias">
                    <RouterLink to="/emergencias-activas">
                        Emergencias Activas
                    </RouterLink>
                </TabsTrigger>

                <!-- Pestaña para Emergencias Finalizadas -->
                <TabsTrigger value="finalizadas">
                    <RouterLink to="/emergencias-finalizadas">
                        Emergencias Finalizadas
                    </RouterLink>
                </TabsTrigger>

                Pestaña comentada para futuras funcionalidades (Consultar Emergencia)
                <TabsTrigger value="consultar">
                    <RouterLink to="/consultar-emergencia">
                        Consultar Emergencia
                    </RouterLink>
                </TabsTrigger> 
            </TabsList>
        </Tabs>
    </div>
</template>
